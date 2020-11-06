# AWK Github Guidelines
This repository stores the guidelines for working with Github at AWK Group. The purpose of this documentation is to provide transparancy and consistency in dealing with coding projects. It describes the desired naming conventions, provides an introduction to basic Git commands, Git Feature Branch Workflow and lists the responsible contact persons.


### Basic Git Commands

Basic git commands and tools can be found in the source folders `git` and `tools` respectively.


### Naming Conventions

Each repository shall follow a distinct naming convention for clarity and ease of findability. Thereby, one distinguishes between customer and internal projects. Furthermore, the naming shall also include the team (Team abbreviation: `DA_AI`, `AI`, `DI` or `ORG`) responsible for the maintenance of the repository.

* Customer: `Projectnumber-Customer_Abbreviation-Projectname` (e.g. *114045046-ASTRA-Fahrzeit*)
* Internal: `Team_Abbreviation-Technology_Platform-Projectname` (e.g. *DA_AI-Jupyter-DataLab_Stack*)


### Best Practices

* Adhere to the Git branching standards (cf. below).
* Do not leak secrets (API keys, login information, etc.) into source code.


### Git Feature Branch Workflow

The core idea behind the Feature Branch Workflow is that all feature development should take place in a dedicated branch instead of the master branch. This encapsulation makes it easy for multiple developers to work on a particular feature without disturbing the main codebase. It also means the master branch will never contain broken code, which is a huge advantage for continuous integration environments. 

![Git Feature Branch Workflow](https://wac-cdn.atlassian.com/dam/jcr:09308632-38a3-4637-bba2-af2110629d56/07.svg?cdnVersion=1320)

For more information, refer to the following documentation by Bitbucket: 

* [Introduction to Git Feature Branch Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow)

Single collaborator projects (that do not go into production) and documentation repos (like this one) do not need to follow strict branching standards.


### Planned Extensions of AWK Github

- [ ] Github Enterprise for SSO, continuous integration, testing and delivery?


### Contact Persons

* Thomas Kathriner (thomas.kathriner@awk.ch) - CoP Data Analytics & Artificial Intelligence
* Jesko Mueller (jesko.mueller@awk.ch) - CoP Digital Infrastructures