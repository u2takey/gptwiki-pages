# guptime 
## chatgpt 
guptime 是一个 Python 的第三方库，用于获取系统的运行时间和负载。它使用了 /proc/stat 和 /proc/uptime 这两个系统 proc 文件的内容。这个库需要在 Linux 环境下使用。

具体来说，guptime 可以返回以下信息：

- uptime: 系统运行时间
- current_time: 当前时间
- uptime_since_timestamp: 系统运行时间距离某个时间戳的秒数
- boot_time: 系统启动时间
- load_average_1min: 1 分钟的平均负载
- load_average_5min: 5 分钟的平均负载
- load_average_15min: 15 分钟的平均负载
- num_processors: 处理器个数

这些信息可以通过 guptime.uptime() 方法获取。

除了 uptime 方法之外，还有以下方法：

- load_average(): 返回一个元组，包含 1 分钟、5 分钟和 15 分钟的平均负载
- stats(): 返回一个字典，包含系统运行时间、当前时间和负载等信息

guptime 可以用于监控系统的负载和运行时间，方便管理者进行调优和监控。 

## tldr 
 
> 这是 `-p linux uptime` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux uptime`
