FGBuildTutorialAndroid
---

Simple template-like gradle build script for android projects. Designed
so that all product variants get checked for coding styles and coding grammar
while only the main sourceSet gets analyzed for NCSS stats and the debug
variant is analyzed for cyclic defects.

This will be kept up-to-date as the android gradle plugin and 3rd party plugins
change.

# Aim of System

To build artifacts of the software application or library and their documentations
and collect OOP meaningful stats. Its not the tools, its the knowledge-theory
of why you should put them together in your own build process.

# Inspiration

W E Deming and W Shewhart

# Usage

For the app module modify build.gradle in app module to suit. For a library
module remove the rename apk and copy apk tasks out of the android.applicationVariants.all
block and change the block name to android.libraryVariants.all

# IDE Specifics

For documentation purposes you might like UML diagrams. On the IntelliJ IDE you can
use the COde Iris plugin which produces a nice png file of UML diagrams.

Obviously, the mirror plugin that mirrors the android UI is a nice addition too.
However, its not free as you have to pay for it.

# Gradle Plugins Used

## Spoon

## hugo

## loglifecycle



# License

# Credits

Credits go to the creator of Gradle and the Google Engineers.