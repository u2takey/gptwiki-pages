# gtimeout 
## chatgpt 
gtimeout是一个Linux命令，它用于在特定时间内运行另一个命令，如果命令在该时间内没有完成执行，则gtimeout命令将终止该命令的执行。gtimeout命令的语法如下：

```
gtimeout [OPTION] DURATION COMMAND [ARG]...
```

其中，OPTION是指gtimeout命令的选项，DURATION是指命令运行的时间限制（单位为秒），而COMMAND和ARG是指要限制运行时间的命令及其参数。

gtimeout命令的常用选项如下：

- -s, --signal=SIGNAL：指定在超时时要发送给命令的信号
- -k, --kill-after=DURATION：指定超时后要等待的时间（单位为秒）后强制终止命令的执行
- -h, --help：显示gtimeout的帮助信息

例如，要限制sleep命令的执行时间为5秒，可以使用以下gtimeout命令：

```
gtimeout 5s sleep 10s
```

在此命令中，gtimeout将sleep命令的执行时间限制为5秒，因此在5秒时间到达时，gtimeout将强制终止sleep命令的执行。 

## tldr 
 
> 这是 `-p linux timeout` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux timeout`
