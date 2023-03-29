# docker 
## chatgpt 
docker命令是Docker CLI（命令行工具）的主要命令。它提供了许多用于管理和运行Docker容器、镜像和网络的子命令。

以下是一些常用的docker命令：

1. docker run：用于运行Docker容器。可以使用该命令指定容器的名称、镜像名称、端口映射、环境变量等。

2. docker pull：用于拉取（下载）Docker镜像。

3. docker build：用于构建Docker镜像。可以使用该命令指定Dockerfile文件以及其他构建参数。

4. docker images：用于列出所有可用的Docker镜像。

5. docker ps：用于列出正在运行的Docker容器。

6. docker stop：用于停止正在运行的Docker容器。

7. docker rm：用于删除已停止的Docker容器。

8. docker rmi：用于删除Docker镜像。

9. docker exec：用于在运行的Docker容器内部执行命令。

10. docker logs：用于查看Docker容器的日志。

除了这些常用的子命令外，docker还有许多其他有用的子命令，如docker-compose、docker swarm等。

总之，docker命令是Docker生态系统中非常重要的一部分，它提供了强大的工具来管理并运行Docker容器和镜像。 

## tldr 
 
> 管理 Docker 容器和镜像。
> 此命令也有关于其子命令的文件，例如：`docker run`.
> 更多信息：<https://docs.docker.com/engine/reference/commandline/cli/>.

- 列出目前正在运行的 docker 容器：

`docker ps`

- 列出所有 docker 容器（包括停止的容器）：

`docker ps -a`

- 透过镜像启动容器，并为容器命名：

`docker run --name {{容器名称}} {{镜像}}`

- 启动或停止现有容器：

`docker {{start|stop}} {{容器名称}}`

- 从 docker registry 中拉取镜像：

`docker pull {{镜像}}`

- 从正在运行的容器内打开一个 shell：

`docker exec -it {{容器名称}} {{sh}}`

- 删除一个停止的容器：

`docker rm {{容器名称}}`

- 获取并查看容器的日志：

`docker logs -f {{容器名称}}`
