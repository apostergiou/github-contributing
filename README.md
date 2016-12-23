# Contribution Guidelines

1. [Prerequisites](#prerequisites)
2. [Forking the project](#forking-the-project)
3. [Create a branch](#create-a-branch)
4. [Run the tests](#run-the-tests)
5. [Commit changes](#commit-changes)
6. [Create a pull request](#create-a-pull-request)

## Prerequisites

Usually every project has its special guidelines for contributing. Always follow these guidelines.
If your contribution is relatively big or a feature, first open an issue to discuss this and get approval. Then, start the feature development.

## Forking the project

1. [Fork](https://help.github.com/articles/fork-a-repo/) the repository.

2. [Clone](https://help.github.com/articles/cloning-a-repository/) your fork.

  ```shell
  git@github.com:apostergiou/github-contributing.git
  ```

## Create a branch

Start a new branch for your feature/change. Remember to follow the project's naming conventions for the feature branch.

```shell
git branch refactor-code # remember to respect repo naming conventions for branches
```

## Run the tests

Make sure your changes don’t break the existing project. Test your changes with the existing suite and if possible add tests for your changes.

e.g. [RSpec](https://github.com/rspec/rspec):
  ```shell
  rspec
  ```
## Commit changes

Commit your changes. Follow the [git-stye-guide](https://github.com/agis-/git-style-guide#commits).

```shell
git commit -m "Refactor code"
```

## Create a pull request

Once your commits are squashed into small logical changes, go ahead and open a pull request. Adding a comment describing your feature, will usually help the review process.

Simply push to origin and use the new pull request button.

```shell
git push origin refactor-code
```

### Renaming your remote feature branch

An easy way to do this is the following:

1) Create a new branch(execute this from your old-branch)

`git branch new-branch origin/old-branch`

2) Push your branch with its brand new name to origin:

`git push origin --set-upstream new-branch`

3) Delete the old branch from origin and the local machine:

`git push origin :old-branch`
`git branch -D old-branch`

## Resources

- See [Free Code Camp](https://github.com/FreeCodeCamp/how-to-contribute-to-open-source) for a more detailed real world guide.
- Github Guides
  - [Contributing to Open Source](https://guides.github.com/activities/contributing-to-open-source/)
  - [Forking Projects](https://guides.github.com/activities/forking/)
  - [Be Social](https://guides.github.com/activities/socialize/)
  - [Mastering Issues](https://guides.github.com/features/issues/)
- Begginer's Guides
  - [General Guide](http://lornajane.net/posts/2010/contributing-to-projects-on-github)
  - [Beginner's Guide](https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/)
  - [Git Style Guide](https://github.com/agis-/git-style-guide)
