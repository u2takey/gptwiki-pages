# glogger 
## chatgpt 
glogger是一个用于记录系统日志的工具。它读取系统日志（通常是/var/log/messages文件）并将日志输出到指定的文件或Syslog服务器。可以使用glogger命令在命令行中运行此工具。

下面是glogger命令的基本语法：

```
glogger [options] message
```

其中message是要记录的日志消息。options包括：

- -h：显示帮助信息。
- -s：指定Syslog服务器。
- -p：指定Syslog服务器的端口。
- -t：指定日志消息的标签（通常是进程名）。
- -f：指定要记录到的文件名。
- -n：在Syslog服务器上使用DNS（默认情况下使用IP地址）。

例如，以下命令将日志消息“Test message”记录到/var/log/test.log文件中：

```
glogger -f /var/log/test.log "Test message"
```

使用glogger命令可以将系统日志记录到运维工程师所在的日志分析平台上，方便问题分析和故障排除。 

## tldr 
 
> 这是 `-p linux logger` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux logger`
