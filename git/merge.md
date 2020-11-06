Merge
===

Commands
---
**git merge [\<options\>] [\<refspec\>]**\
**git merge \-\-abort | \-\-continue**

Description
---
Incorporate changes that occured between when the given **refspec** diverged from the current branch into it.

**Warning**: Running git merge with non-commited and/or non stashed changes is to be avoided at all costs.\
Git might not be able to restore if the merge is aborted.

Most commonly used options
---
* **-m**: specify the merge message
* **\-\-ff**: only update the branch pointer without creating a merge commit\
    This is the default behaviour.
* **\-\-no-ff**: create a merge commit even if the merge resolves as a **ff**
* **\-\-commit**: perform the merge and commit the result
* **\-\-no-commit**: do not immediatly commit the merge commit after performing the merge.\
    This allows the user to tweak the it.\
    This option doesn\'t do anything on a **ff** merge since there is no merge commit to be done.
* **\-\-squash**: create a single commit on top of the current branch containing the whole merge.
* **\-\-no-squash**: do not squash the commits. This is the default behaviour.

**\-\-no-X** options override their **\-\-X** counterparts

Options during merge
---
* **\-\-abort**: aborts the merge and restores the repository to its previous state
* **\-\-continue**: if the conflicts are marked as resolved, proceeds to the next commit

*As always, the man has more informations especially on merge commits handling and merge strategies.*\
*This man is the most important since it explains how conflicts work and the many nuances of merge strategies*
