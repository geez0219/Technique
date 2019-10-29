## show all docker images
```
docker images
```

## download docker image from docker hub
```
docker pull <repo>/<image>:<tag>
```

## show all container including exit one
```
docker container ls -a
```
```
docker ps -a
```

## start a container (make a container active)
```
docker container <container_name> start 
```

## stop a container
```
docker container <container_name> stop
```

## attach to a container (seldom used)
```
docker container attach <container_name>
```

## go into that container 
```
docker exec -it <container_name> bash
```

## start an container 
```
[docker/nvidia-docker] run -it --name <container_name> -v <source_dir>:/<target_dir> <image_name> bash
```

