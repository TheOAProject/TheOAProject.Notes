# The OA Project Notes



## About project

Сross-platform notes service. This service can be installed on a dedicated VPC server(or deploy a docker image) and used as a personal notes service. The advantages of this service are that it can be used on any platform with instant synchronization.

## Build info
Azure Build Status (master)/(dev)

| master   |  dev   |
|----------|-------------|
| [![Build Status](https://dev.azure.com/o2bionics-products/TheOAProject/_apis/build/status%2FTheOAProject.Notes?branchName=master)](https://dev.azure.com/o2bionics-products/TheOAProject/_build/latest?definitionId=65&branchName=master) | [![Build Status](https://dev.azure.com/o2bionics-products/TheOAProject/_apis/build/status%2FTheOAProject.Notes?branchName=dev)](https://dev.azure.com/o2bionics-products/TheOAProject/_build/latest?definitionId=65&branchName=dev) |

GitHub

| master   |  dev   |
|----------|-------------|
| [![TheOAProject.Notes](https://github.com/TheOAProject/TheOAProject.Notes/actions/workflows/github-ci.yml/badge.svg?branch=master)](https://github.com/TheOAProject/TheOAProject.Notes/actions/workflows/github-ci.yml) | [![TheOAProject.Notes](https://github.com/TheOAProject/TheOAProject.Notes/actions/workflows/github-ci.yml/badge.svg?branch=dev)](https://github.com/TheOAProject/TheOAProject.Notes/actions/workflows/github-ci.yml) |


## **Preinstalled software**
### Windows:
- [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/) or [Microsoft VS Code](https://visualstudio.microsoft.com/downloads/)
- [Microsoft SQL Server or Docker image with (minimal version version 2019 and up)](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) 
- [.Net Core 8](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)

### Mac
- [Visual Studio 2022 for Mac](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio-mac/?sku=communitymac&rel=17) or [Microsoft VS Code](https://visualstudio.microsoft.com/downloads/)
- [.Net Core 8](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)
- Intel
    - [Microsoft SQL Server or Docker image with (minimal version version 2019 and up)](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) 
- or Apple Silicon
    - [Azure SQL Edge](https://learn.microsoft.com/en-us/azure/azure-sql-edge/disconnected-deployment)

### Linux
- [Microsoft VS Code](https://visualstudio.microsoft.com/downloads/)
- [.Net Core 8](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)

## Commit Formats
#### Types
* API relevant changes
    * `feat` Commits, that adds a new feature
    * `fix` Commits, that fixes a bug
* `refactor` Commits, that rewrite/restructure your code, however does not change any behaviour
    * `perf` Commits are special `refactor` commits, that improves performance
* `style` Commits, that do not affect the meaning (white-space, formatting, missing semi-colons, etc)
* `test` Commits, that add missing tests or correcting existing tests
* `docs` Commits, that affect documentation only
* `build` Commits, that affect build components like build tool, ci pipeline, dependencies, project version, ...
* `devops` Commits, that affect operational components like infrastructure, deployment, backup, recovery, ...
* `chore` Miscellaneous commits e.g. modifying `.gitignore`

#### Subject
* use imperative, present tense (eg: use "add" instead of "added" or "adds")
* don't use dot(.) at end
* don't capitalize first letter

### Examples
* ```
  feat(service): add and setup swagger
  ```
* ```
  feat: remove ticket list endpoint
  
  refers to JIRA-999
  BREAKING CHANGES: ticket enpoints no longer supports list all entites.
  ```
* ```
  fix: add missing parameter to service call
  
  The error occurred because of <reasons>.
  ```
* ```
  build(release): bump version to 1.0.0
  ```
* ```
  build: update dependencies
  ```
* ```
  refactor: implement calculation method as recursion
  ```
* ```
  style: remove empty line