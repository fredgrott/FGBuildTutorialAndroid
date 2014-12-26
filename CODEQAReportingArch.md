CODEQAReportingArch
---

As of android gradle plugin 1.x we do not have an easy way to setup codeqa
analysis and reporting via the normal gradle way of sourcesets as
java sourcesets and android.sourceSets are different in that we
do not have outputs as we only have outputs via the Variants collection.

But, we still have an immediate need to analyze and report codeqa
in such a way that we analyze  the productFlavor variants.

# Solution

Parts of the solution are:

1. Manually set checkstyle and pmd and javancss to analyze source of all variants.
2. Manually set jdepend to analyze debug as that is the default variant buildType
   that gets compiled by the IDE.
3. If we need additional Jdepend analysis on another variant buildType than it needs
   to be setup in a gradle.taskGraph.whenReady DAG block hasTask(release) for example
   so that the task only gets created if release task is being executed and thus
   produces jdepend analysis for he release buildType variant.
4. Separate out tasks so that jdepend gets executed first and than checkstyle, pmd,
   and javancss so that when it comes time to complete the xslt transforms
   the jdepend xml file is not null.
5. group xslt transforms into one aggregate task for final html report generation.
6. Add the appropriate xsl parameters for things like project name, individual developer name,
   build time, etc.
7. Since groovy distros contain the jetty web container we can create a groovy
   dash board that can get launched via ant.taskdefs to than create a
   dash board summary of al the reports and individual htnml reports.
   At that time we can eliminate the task created in step 5 as being no longer needed.


# CodeQA Non-Dashboard Xsl Parameter Scheme

Parameters:

project
module
rulesets
today
time
context