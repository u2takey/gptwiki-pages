# launchd 
## chatgpt 
launchd是Mac OS X和其他UNIX操作系统上的守护进程管理器，它是在操作系统启动时启动的第一个进程。它负责启动和管理所有系统服务、守护进程和用户进程。

以下是launchd的一些常见应用：

1.启动系统服务 – launchd启动了操作系统中的所有服务，例如web服务器、DNS服务器和文件共享服务器。

2.运行守护进程 – launchd可以启动由系统和应用程序创建的守护进程。例如，launchd可以运行一个定期备份操作。

3.运行周期性任务 – launchd可以启动周期性的任务，例如定期清理磁盘空间或运行负载测试。

launchd可以理解为一种管理服务的工具，可以并行启动多个服务以及它们的子服务，还可以监控这些服务的运行状态，一旦发现它们运行失败或因某些原因停止运行，launchd会自动尝试重新启动它们，最大限度地减少人为干预，提高系统的稳定性和可靠性。该命令在维护Mac OS X和其他UNIX操作系统中的系统稳定性和可靠性方面发挥着重要作用。 

## tldr 
 
> 这是 `launchctl` 命令的一个别名。
> 更多信息：<https://developer.apple.com/library/archive/documentation/MacOSX/Conceptual/BPSystemStartup/Chapters/Introduction.html>.

- 原命令的文档在：

`tldr launchctl`
