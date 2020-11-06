# AWK Github Guidelines
This repository stores the guidelines for working with Github at AWK Group. The purpose of this documentation is to provide transparancy and consistency in dealing with coding projects. It provides an introduction to Gitflow, describes the desired naming conventions and lists the responsible contact persons.


## Gitflow Workflow

The goal is to encapsulate feature development in order to not disturb the main codebase. Instead of commiting to the master branch, developers create a seperate branches for a new features. In this context, Gitflow is a suggested workflow for managing larger projects with scheduled release cycle. Specifically, it assigns specific roles and interaction rules to different types of branches.

**Develop and Master Branches**

There are two branches to record the history of the project. The master branch stores the official release history (tagged with a version number), while the develop branch is used for integration of new features. At the beginning of a project, a parallel develop branch can be created locally and pushed to the server by the following bash command.

```console
git branch develop git push -u origin develop
```

**Feature Branches**

New features should reside in their own branches, which can be pushed to the central repository for backup and collaboration. Here, they should use develop as their parent branch. 

```console
git checkout develop git checkout -b feature_branch
```

After a feature is completed, the corresponding feature branch gets merged back into develop.

```console
git checkout develop git merge feature_branch
```

**Release Branches**


## Naming Convention

## Best Practices

## Extensions of AWK Github

## Contact Persons

* Thomas Kathriner (thomas.kathriner@awk.ch)
* Jesko Mueller (jesko.mueller@awk.ch)