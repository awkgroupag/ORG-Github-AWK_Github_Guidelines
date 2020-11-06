Push
===

Command
---
**git push [\<repository\> [\<refspec\>]]**

where:

* **repository** is the remote repository that is the destination of the push (usually *origin*)
* **refspec** is the target remote ref

Description
---
updates remote refs using local refs.

example: *git push origin master*\
    pushes on the ref master of the origin remote.


Most commonly used options:
---
* **\-f, \-\-force**: forces the push\
(which usually fails if the branch\'s local history differs with the remote\'s history)

*As always, the man has more informations*
