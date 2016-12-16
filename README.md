# Contribution Guidelines

1. [Prerequisites](#prerequisites)
2. [Forking the project](#forking-the-project)
3. [Create a branch](#create-a-branch)
4. [Make changes](#make-changes)
5. [Run the tests](#run-the-tests)
6. [Squash your commits](#squash-your-commits)
7. [Create a pull request](#create-a-pull-request)
8. [Garden your branches](#garden-your-branches)

## Prerequisites

Usually every project has its special guidelines for contributing. Always follow these guidelines.

## Forking the project

1. [Fork](https://help.github.com/articles/fork-a-repo/) the repository.
2. [Clone](https://help.github.com/articles/cloning-a-repository/) your fork.

## Create a branch

Start a new branch for your feature/change. Remember to follow the project's naming conventions for the feature branch.

## Make changes

## Run the tests

## Squash your commits

## Create a pull request


## Resources

- See [Free Code Camp](https://github.com/FreeCodeCamp) for a more detailed real world guide.
- Must read [guide](https://github.com/FreeCodeCamp/how-to-contribute-to-open-source).

## Garden your branches

### Renaming your remote feature branch

An easy way to do this is the following:

1) Create a new branch(execute this from your old-branch)

`$ git branch new-branch origin/old-branch`

2) Push your branch with its brand new name to origin:

`$ git push origin --set-upstream new-branch`

3) Delete the old branch from origin and the local machine:

`$ git push origin :old-branch`
`$ git branch -D old-branch`
