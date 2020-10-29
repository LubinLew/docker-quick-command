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