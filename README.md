# Contribution Guidelines

- [Prerequisites](#prerequisites)
- [Forking the project](#forking-the-project)
- [Upstream and Origin](#upstream-and-origin)
- [Create a branch](#create-a-branch)
- [Run the tests](#run-the-tests)
- [Commit changes](#commit-changes)
- [Squash commits](#squash-commits)
- [Create a pull request](#create-a-pull-request)

## Prerequisites

Usually every project has its special guidelines for contributing. Always follow these guidelines.
If your contribution is relatively big or a feature, first open an issue to discuss this and get approval. Then, start the feature development.

## Forking the project

1. [Fork](https://help.github.com/articles/fork-a-repo/) the repository.

2. [Clone](https://help.github.com/articles/cloning-a-repository/) your fork.

  ```shell
  git clone git@github.com:apostergiou/github-contributing.git
  ```

## Upstream and Origin

See http://stackoverflow.com/questions/9257533/what-is-the-difference-between-origin-and-upstream-on-github.

- `upstream` generally refers to the original repo that you have forked. Use `upstream` to fetch from the original repo (in order to keep your local copy in sync with the project you want to contribute to).

- `origin` is your fork: your own repo on GitHub, clone of the original repo of GitHub. Use `origin` to pull and push since you can contribute to your own repo.

From the GitHub page:

> When a repo is cloned, it has a default remote called origin that points to your fork on GitHub, not the original repo it was forked from.
To keep track of the original repo, you need to add another remote named upstream

```shell
git remote add upstream git://github.com/original-project/repo.git
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

## Squash commits

```shell
$ git fetch upstream
$ git checkout my-feature
$ git rebase -i upstream/master

# choose squash for all of your commits, except the first one
# Edit the commit message to make sense, and describe all your changes

$ git push origin my-feature -f
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
  - [How to write the perfect pull request](https://github.com/blog/1943-how-to-write-the-perfect-pull-request/)
