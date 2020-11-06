Rebase
===

Commands
---
**git rebase [-i] [options] [\-\-onto newbase] [upstream [branch]]**

**git rebase \-\-continue | \-\-skip | \-\-abort**


Description
---
If **branch** is specified, rebase will checkout on it before doing anything else.

The branch is reset (similarly to a *git reset --hard*) onto **upstream** (or **newbase** if provided).

The commits between **upstream** and the previous HEAD of **branch** are then reapplied on the branch.
Commits that were already present on the branch (same changes, different message or timestamp) are ignored.

It is *very* recommended to stash your changes before performing a rebase.

During a rebase, if you make some changes on a commit you'll have to stage said changes and edit it using **git commit \-\-amend**

The examples from the man are really neat.

Most commonly used options:
---
* -i, \-\-interactive: enable the interactive mode allowing the user to specify what to do with each commit.

Most commonly used options during rebase
---
* \-\-continue: Confirm the changes on a commit and proceed to rebase the next
* \-\-skip: If there are no changes tracked by git, proceed to rebase the next commit.
* \-\-abort: Abort the rebase and reset the repository to it\'s original state.

*As always, the man has more information*
