# Revert master branch to upstream

_(Source: http://stackoverflow.com/a/8135023/1396155)_

(I'm assuming that the changes that you now want to ignore are at your origin remote, you're on your master branch, and you want to revert to the contents of the upstream remote)

Firstly, reset your working copy to the upstream master:

```
git remote update
# the double hyphen ensures that upstream/master is
# considered as a revision and not confused as a path
git reset --hard upstream/master --
```

Then push this new branch-head to your origin repository, ignoring the fact that it won't be a fast-forward:

```
git push origin +master
```
