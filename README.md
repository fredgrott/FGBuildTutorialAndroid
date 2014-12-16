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

[W E Deming](http://en.wikipedia.org/wiki/W._Edwards_Deming) and [W Shewhart](http://en.wikipedia.org/wiki/Walter_A._Shewhart), cofathers of the QA and SPC movement in the US.
If you have never heard of these two people, it might be a good idea to do some reading.

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

[spoon](https://github.com/stanfy/spoon-gradle-plugin)

Developed by Stanfy corp.


## hugo

[hugo](https://github.com/JakeWharton/hugo)

Developed by Jake Wharton, use by annotating:
        @DebugLog



## loglifecycle

[loglifecycle](https://github.com/stephanenicolas/loglifecycle)

Developed by Stephane Nicolas. Use by simply annotating activity, fragments, service, views:
           @LogLifecycle



# License

Copyright 2014 Fred Grott(GrottWorkShop)

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

# Credits

Credits go to the creator of Gradle and the Google Engineers.