FGBuildTutorialAndroid
---

This is a Gradle Build Tutorial for Android Java Application development. The general idea
is include tips and best practices so you  the beginning android java application developer
can get up to speed fast and on to coding.

# Architecture

We have some use cases where things change from no product flavors to product flavors than
to product flavors with flavor groups. The things changing is aspects of the apk, javadocs,
etc such as file names,etc.  Thus, the idea is to get one block of code that handles
all these use cases and than our build script becomes two major components that for most
cases can be copied for all our uses.

Project modules app and library are single developer mode build scripts in that they
have certain single developer project assumptions. For projects with multiple developers
and having access to a continuous build integration server you would remove the
automatic jarring of the release doc,zip of docs, and the zipping of the release and
proguard mapping files and archiving them at the subfolder archive at project root folder.


# License

Build scripts and code is license under the Apache 2.0 License.
If you as a beginning android developer find this useful I would appreciate if
you would mention it on:

[RedditAndroidDev]()



# Credits

Credits go to the devs that came up with Groovy and Gradle and the ADT-Dev Google Engineers and
the independent 3rd part code committers to the ADT tool-set and of course to the IntelliJ
team for making an open source version of their fine IDE.

# Resources

[Android Gradle Plugin Doc]()

[Gradle Docs download]()


