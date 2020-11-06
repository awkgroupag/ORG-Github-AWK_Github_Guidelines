Gitignore
===

Description
---
This feature allows the user to make git ignore pathes.\
It is handled by the **.gitignore** file located at the root of the repository.

Comments start with **#**\
Blank lines are ignored

[This](https://www.gitinore.io) tool is pretty usefull.

wildcards
---
They\'re pretty much standard

* **\'\*\'**: any characters except '/' and '?'
* **\'?\'**: any character except '/'
* **\[***things***\]**: any of the characters specified
* leading **\"\*\*/\"**: match in all directories
* trailing **\"/\*\*\"**: match everything inside the directory

examples
---
* **\"a/\*\*/b"** matches *\"a/b\"*, *\"a/x/b\"*, and *\"a/x/y/b\"*
* **\"\*\*/foo\"** matches *\"foo\"*, *\"x/foo\"*, and *\"x/y/foo\"*
* **\"bar/\*\*\"** matches *\"bar/x\"* and *\"bar/y/z\"* plus all their children
* **\"\*\*/baz/\*\*\"** matches any directory named baz, wherever it is located, and all of its children.

*As always, the man has more information*
