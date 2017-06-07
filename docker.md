#### Stop / remove all Docker container

```bash
$ docker stop $(docker ps -a -q)
$ docker rm $(docker ps -a -q)
```



