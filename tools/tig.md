TIG
===

TIG is a graphical tool allowing to manage commit creation, stashes, and searching in the log.

It works on linux and is built upon ncurse.

For commit messages, TIG uses the command given the $EDITOR env variable.

Most useful shortcusts:
---
* *main screen*:
    * **h**: display the help screen
    * **S**: show the staging area
    * **C**: cherry-pick a commit
    * **!**: revert a commit
* *staging screen*:
    * **k, l**: navigate in a file
    * **u**: stage or unstage a file
    * **1**: stage or unstage a line
    * **!**: revert a change

*The help screen is more complete and contains many more commands*
