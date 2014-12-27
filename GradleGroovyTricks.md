GradleGroovyTricks
---

# GStrings

To get variable expansion you have to use double quotes and
ant builder will not understand GStrings. Thus, for anything touching
ant builder do a local variable in the ext code block to use
GStrings and get variable expansion.

