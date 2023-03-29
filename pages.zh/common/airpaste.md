# airpaste 
## chatgpt 
airpaste 是一个无线网络传输工具，用于在两个设备之间转换数据。它可以在 Linux 和 macOS 系统上使用。 

airpaste 命令通过 Wi-Fi 传输数据，并且不需要连接到一个路由器或者接入点。使用 airpaste 传输数据时，它会在本地创建一个 Wi-Fi 网络并加密传输数据。 

以下是 airpaste 命令的常用选项和参数：

- `--help`: 显示 airpaste 命令的帮助文档。
- `-l [port]`: 监听指定端口号。默认情况下，airpaste 监听 1337 端口。
- `-s [ip] [port]`: 发送数据到指定 IP 地址和端口号。
- `-c [ip] [port]`: 监听指定 IP 地址和端口号。 

以下是一些使用 airpaste 命令的示例：

- 在两个设备之间传输文件
```
# 接收端
$ airpaste -l | tar -xzvf -

# 发送端
$ tar -czvf test.tar.gz test_folder/ | airpaste -s localhost
```

- 监听指定端口号，接收来自网络上的数据
```
$ airpaste -l 3000
```

- 将数据发送到另一个设备
```
$ echo "Hello World" | airpaste -s 192.168.0.100 3000
```

总的来说，airpaste 命令是一个非常有用的无线网络传输工具，可以轻松地在两个设备之间快速传输数据。 

## tldr 
 
> 在同一网络下共享信息和文件。
> 更多信息：<https://github.com/mafintosh/airpaste>.

- 等待接收消息并显示接收到的信息：

`airpaste`

- 发送文本：

`echo {{文本}} | airpaste`

- 发送文件：

`airpaste < {{文件的路径}}`

- 接收文件：

`airpaste > {{文件的路径}}`

- 创建 / 加入频道：

`airpaste {{频道名}}`
