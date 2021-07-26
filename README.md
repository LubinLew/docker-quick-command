# docker-quick-command

## docker-tags

```bash
Usage: docker-tags NAME[:TAG]

docker-tags list all tags for docker image on a remote registry.

Example:
    docker-tags (default nginx)
    docker-tags nginx
    docker-tags nginx:1.15.8
    docker search nginx | docker-tags
    docker search nginx | docker-tags :1.15.8
    echo nginx | docker-tags
    echo nginx | docker-tags :1.15.8
```

## delete all none version

```bash
docker images | awk '$2 ~/<none>/{print $3}'|xargs docker rmi
```

## delete all history

```bash
docker rm `docker ps -a -q`
```
