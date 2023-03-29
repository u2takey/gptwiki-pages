# docker build 
## chatgpt 
docker build 命令用于在本地环境中构建一个新的Docker镜像。该命令会根据指定的 Dockerfile 和上下文路径（构建上下文）来创建镜像。具体地，该命令的语法为：

```
docker build [OPTIONS] PATH
```

其中，OPTIONS 可选，用于指定构建时的各种参数和选项；PATH 是构建上下文的路径，即 Dockerfile 等构建所需文件所在的目录。

以下是一些主要的 OPTIONS 选项：

- -t, --tag: 指定新镜像的名称及标签。格式为 [name:tag]，其中 name 为镜像名称，tag 为镜像的版本号，如果省略 tag，则默认为“latest”。
- --build-arg: 指定构建时的参数，格式为 key=value。
- -f, --file: 指定 Dockerfile 文件路径。默认情况下，该命令会在构建上下文中寻找名为 Dockerfile 的文件。
- --no-cache: 表示不使用缓存，从头开始构建镜像。
- -m, --memory: 指定构建时使用的内存限制，格式为整数+单位（如100m）。

例如，以下命令用于在当前目录下的 Dockerfile 和上下文中构建名称为 myimage 的镜像，并打上 v1.0 的标签：

```
docker build -t myimage:v1.0 .
```

该命令会将 Dockerfile 和构建上下文中的所有文件打包成一个新的镜像，用于发布和部署应用程序。 

## tldr 
 
> 从 Dockerfile 打包镜像。
> 更多信息：<https://docs.docker.com/engine/reference/commandline/build/>.

- 使用当前目录下的 Dockerfile 打包一个 docker 镜像：

`docker build .`

- 从指定 URL 的 Dockerfile 打包 docker 镜像：

`docker build {{github.com/creack/docker-firefox}}`

- 打包一个 docker 镜像并指定镜像的标签：

`docker build --tag {{name:tag}} .`

- 打包一个没有上下文的 docker 镜像：

`docker build --tag {{name:tag}} - < {{Dockerfile}}`

- 打包镜像时不使用缓存：

`docker build --no-cache --tag {{name:tag}} .`

- 使用指定的 Dockerfile 打包一个 docker 镜像：

`docker build --file {{Dockerfile}} .`

- 传入自定义变量用于打包：

`docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .`
