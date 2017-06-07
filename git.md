#### Remove all local git branches

```
$ git branch --no-color --merged master | grep -v master | grep -v \* | xargs git branch -d
```



