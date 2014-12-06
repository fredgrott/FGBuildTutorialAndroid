FGBuildTutorialAndroid
---

This is a Gradle Build Tutorial for Android Java Application development. The general idea
is include tips and best practices so you  the beginning android java application developer
can get up to speed fast and on to coding.

# Architecture

## 1.0.x (android gradle plugin versions)

1. The Android Gradle Plugin does not load the full set of java plugins. Effects are that your codeqa
   plugins that are default with gradle DO NOT auto-generate per sourceSets and thus you
   are forced to dynamically create them. Also, its an android sourceSet who's underlying
   API is not yet fully aligned with the Gradle Java sourceSet API as of yet for
   android gradle plugin versions 1.0.x.

2. DSL for things like sourceSets, etc is still undocumented in certain places.

Thus, my best best practices guesses when in undocumented areas was to search
Google for notes from some recognized Google Engineers that happen to be on
the Android Tools dev team.

THE MOST STABLE BLOCK

Obviously, the android block is the most stable with next-to-almost no guesses
thus other than minor plugin version changes that andorid block will stay
somewhat the same across android gradle minor plugin version.

THE INTERMEDIATE STABLE BLOCK

The project.afterEvaluate block is where my best guesses are contained. The guesses are
constrained with some groovy to prevent a full-blown blow-up when we run into
dsl changes via the android gradle plugin minor versions. Meaning,
every once-in-awhile you might have to change something but not too much.


## 1.1.x (android gradle plugin versions)



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


