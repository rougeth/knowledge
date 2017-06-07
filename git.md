# Remove all local git branches

```
$ git branch --no-color --merged | grep -v master | grep -v \* | xargs git branch -d
```

1. List all local branches. `--merged`  filter branches that were already merged into a specific branch \(master by default\) and `--no-color  a` turn off branch colors, useful for later filtering with grep.  
   `git branch --no-color --merged`

2. Filter protected branches with \`grep -v &lt;pattern&gt;\`.

3. Use `xargs` to send the output of the first command as arguments to `git branch -d` .

References:

* https://git-scm.com/docs/git-branch
* https://git-scm.com/docs/git-branch\#git-branch---mergedltcommitgt
* https://git-scm.com/docs/git-branch\#git-branch---no-color



