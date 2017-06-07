# Stop / remove all Docker containers

```bash
$ docker stop $(docker ps -a -q)
$ docker rm $(docker ps -a -q)
```

1. List containers with  `docker ps`. `-a/--all` include also the stopped ones and `-q/--quiet` display only the numeric IDs.
2. Use `docker stop` and `docker rm` with the output of the first command \(got from bash command substitution\).

References:

* https://docs.docker.com/engine/reference/commandline/ps/
* https://docs.docker.com/engine/reference/commandline/stop/
* https://docs.docker.com/engine/reference/commandline/rm/
* https://www.gnu.org/software/bash/manual/bashref.html\#Command-Substitution



