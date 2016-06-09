# Delete remote branch

_(Source: http://stackoverflow.com/a/2003515/1396155)_

As of [Git v1.7.0](https://github.com/gitster/git/blob/master/Documentation/RelNotes/1.7.0.txt), you can delete a remote branch using

```
git push origin --delete <branchName>
```

which is easier to remember than

```
git push origin :<branchName>
```

which was added in [Git v1.5.0](https://github.com/gitster/git/blob/master/Documentation/RelNotes/1.5.0.txt) "to delete a remote branch or a tag."

***

[Go back](README.md)
