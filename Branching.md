# Branching

We use [http://nvie.com/posts/a-successful-git-branching-model/](Git Flow
Branching Model). It's a branching strategy that helps organize features,
releases, fixes, etc. We use the [https://github.com/nvie/gitflow](git-flow
extension) to make this easier.

After installing git-flow (brew install git-flow), you can start using the
git-flow library by running

`git flow init`

`Branch name for production releases: [master]`

`Branch name for "next release" development: [develop]`

`How to name your supporting branch prefixes? Feature branches? [feature/]`

`Release branches? [release/] Hotfix branches? [hotfix/] Support branches?`

`[support/] Version tag prefix? []`

Git flow will not make any changes to your repository, it's a wrapper around
existing git commands.

### Feature Development

Start a feature:

`git flow feature start {featureName}`

When you're done with the feature using git flow feature finish {featureName}
will merge your code into develop and delete the branch

### HotFixing Production

`git flow hotfix start {hotFixName}`

When you finish, using git flow hotfix finish {hotFixName} will merge your code
to master and develop, deleting the branch.
