config
---

Normally task that extend gradle reporting such as our code checks and such default to
a:

projectmodule/gradle/config/plugin name/config file

But we want to do it at the project root level so that we Do Not Repeat Ourselves thus
I put a config folder at the project root and define my project root ext properties
accordingly.

