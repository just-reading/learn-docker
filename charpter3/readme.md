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

![logo](https://raw.githubusercontent.com/just-reading/learn-docker/master/charpter3/1.jpg)

```bash
docker container run centos ping -c 5 127.0.0.1
```

- docker没有找到对应的container image
- 从默认docker hub docker.io找到image
- 成功pull image
- 运行 ping

## Listing containers

```bash
docker container ls
```

|Column|Description|
|---|---|
|Container ID| 容器唯一id SHA-256.|
|Image| container的image名字|
|Command|启动container的command|
|Created|创建时间|
|Status|容器状态 (created, restarting, running,removing, paused, exited, or dead).|
|Ports|端口 以及映射的外部端口|
|Names|指定的container的名字可以重复|

删除神器

```bash
docker container rm -f $(docker container ls -a -q)
```

start stop remove

```bash
docker container stop quotes

docker container start quotes

docker container rm quotes
```

## Inspecting containers

```bash
docker container inspect quotes
```

## Exec into a running container

```bash
docker container exec -i -t quotes /bin/sh

docker container exec quotes ps
```

## Attaching to a running container

```bash
docker container attach quotes
```

## Container Log

```bash
docker container logs quotes
```