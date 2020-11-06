Stash
===

Commands
---
**git stash list**\
**git stash show [\<options\>] [\<stash\>]**\
**git stash drop [\<stash\>]**\
**git stash (pop | apply) [<\stash\>]**\
**git stash [push] [\<options\>] [\-\-] [\<pathspec\>...]**\
**git stash clear**\

Description
---

Allows the manipulation of stash entries.\
A stash entry stores the state of the working directory and resets it to **HEAD**.

If no **stash** is specified on a command **stash@{0}** (the last stash created) is assumed.

If no operation is specified, **push** is taken as a default.\
If no **pathspec** is given to a **push** operation, the whole working directory is stashed.

Most commonly used options
---

* *list*: list the stash entries
* *show*: show the contents of a stash
    * **-v**: trigger verbosity (show edits in files)
* *push*: create a new stash entry
    * **-m, \-\-message**: replace the default message with a given one
    * **\-\-keep-index**: do not stash changess in the index
    * **-u, \-\-include-untracked**: include untracked files
    * **\-\-all**: include untracked and ignored files
* *apply*: add the stashed changes to the working directory.\
The operation fails in case of conflict.
    * **\-\-index**: try to recreate the index.
* *drop*: remove a stash entry
* *pop*: *apply* and then *drop* a stash entry
* *clear*: *drop* all stash entries

*As always, the man has more informations*
