# Git Rules and Workflow

## Workflow: Github flow

Introduction to Github Flow [guides.github.com/introduction/flow](https://guides.github.com/introduction/flow/)

![](/img/ghflow.png)

## Pull Request General Guidelines

* Please check to make sure that there aren't existing pull requests attempting to address the issue mentioned.
* Check for related issues on the issue tracker.
* Non-trivial changes should be discussed on an issue first.
* Let us know you're working on the issue.
* Develop in a topic branch, not master.
* Provide useful pull request description
* Squash your commits.
* Write a good description of your PR.

### Always follow these rules:

* Commit each fix as a separate change.
* Provide useful commit messages.
* Use the imperative mood in the subject line. Eg. `fix login error`, `add config file`, `remove unused code`
* Provide a short commit message in the first line (50-72 character). Looking at the output of `gitk` or `git log --oneline` might help you understand why.
* Reference the git issue on the body of your commit message, never on the first line. Eg:
```
git commit -m 'add login feature
#3'
```
* Don't pollute the log! http://bit.ly/1MDciJG
  * Don't push to master any 'merge messages'
  * Update your local development branch with `git pull --rebase origin master`
  * Always Rebase over merge.

## Git tools

  There are also tools like [Hub](https://hub.github.com/) and [git-extras](https://github.com/tj/git-extras) that facilitate interacting with Github.
  You can leverage these tools to contribute to this repository.


  ## Version Numbers

  [Semver](http://semver.org), except the version roles have the semantic names, "Breaking.Feature.Fix" instead of "Major.Minor.Patch".


  #### Breaking.Feature.Fix

  We don't decide what the version will be. The API changes decide. Version numbers are for computers, not people. Release names are for people.

  ##### Breaking

  Any breaking change, no matter how small increments the Breaking version number. Incrementing the Breaking version number has absolutely no relationship with issuing a release.

  ##### Feature

  When any new feature is added. This could be as small as a new public property, or as large as a new module contract being exposed.

  ##### Fix

  When a documented feature does not behave as documented, or when a security issue is discovered and fixed without altering documented behavior.
