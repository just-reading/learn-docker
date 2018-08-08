# charpter 3

## cover

- Running the first container
- Starting, stopping, and removing containers
- Inspecting containers
- Exec into a running container
- Attaching to a running container
- Retrieving container logs
- Anatomy of containers

## Running the first container

``` bash
docker -v

docker container run alpine echo "Hello World"
```

重复两次运行以上命令 output不同，因为本地已经有alpine这个image

[logo]: https://github.com/just-reading/learn-docker/raw/master/charpter3/1.img "Logo Title Text 2"