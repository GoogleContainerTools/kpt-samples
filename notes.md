# Steps for publishing a package


Assuming you have usual git remotes setup. For example, on my machine:

```sh
kpt-samples $ git remote -v
origin  git@github.com:droot/kpt-samples.git (fetch)
origin  git@github.com:droot/kpt-samples.git (push)
upstream        git@github.com:googlecontainertools/kpt-samples.git (fetch)
upstream        git@github.com:googlecontainertools/kpt-samples.git (push)
```

Let say, your latest iteration on a package (say `ghost`) got merged.

```sh

git checkout main
git fetch upstream
git rebase upstream/main

# ensure you see your change
git log

# ok, all set to publish the package
git tag <pkg-name>/<pkg-version> main
git tag upstream <pkg-name>/<pkg-version>


# Here is how the command looked for publishing ghost v2 package

git tag ghost/v2 main
git tag upstream ghost/v2

```
