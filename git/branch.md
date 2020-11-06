Branch
===

Commands
---
**git branch [\<options\>] [-l | \-\-list]**\
**git branch [\-\-track | \-\-no-track] [-f] \<new-branch\> [start-point]**\
**git branch (-u upstream | \-\-set-upstream-to=upstream) [branchname]**\
**git branch (-c | -C) [\<oldbranch\>] \<newbranch\>**\
**git branch (-m | -M) [\<oldbranch\>] \<newbranch\>**\
**git branch (-d | -D) [\<oldbranch\>] \<newbranch\>**

Description
---
Allows the listing of and operations on branches.

If no options are given **\-\-list** is assumed.\
If a branch name is given, it creates a new branch.

Most commonly used options
---
* **-u, \-\-set-upstream-to=**: set the upstream (parent branch) of the branch
* **--unset-uptstream**: unset the upstream of the specified (default current)
* **\-\-track**: force the setting of the upstream.
* **\-\-no-track**: force not setting the upstream.
* **-f, \-\-force**: force the operation
* **-c, -C**: copy the branch
* **-d, -D**: delete the branch
* **-m, -M**: move the branch

The capital versions of these options imply a **\-\-force**.

Most commonly used list options
---
* **-a, \-\-all**: List both remote tracking and local branches
* **-v, -vv, \-\-verbose**: add verbosity (branch names, sha1, commits...)

*As always, the man has more informations*
