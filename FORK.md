# Fork guide
This file will describe how to bring changes to this repository.
Assuming tonic's main branch was updated, and we want to synchronize this fork, the steps are:
```bash
git remote add upstream https://github.com/hyperium/tonic.git
git fetch upstream master
git checkout git subtree split -P tonic-build -b upstream-tonic-build
git push -u upstream-tonic-build
# PR on github
```