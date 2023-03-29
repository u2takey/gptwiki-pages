# reboot 
## chatgpt 
reboot 命令是 Linux 系统重启的命令。它会向系统发送一个信号，通知系统关闭并重新启动。当您运行 reboot 命令时，系统会立即停止所有运行中的程序、服务、进程和其他任务，并启动系统重新启动过程。因此，您必须谨慎使用 reboot 命令，以免造成数据丢失或其他不良影响。

更具体地说，reboot 命令会执行以下操作：

1. 使用 sync 命令刷新内存缓存中的所有数据，以确保所有数据都被写入磁盘。

2. 写入重启指令到内存的相应位置，并向操作系统内核发送一个信号来通知它启动重启过程。

3. 关闭所有正在运行的进程和服务，以确保它们的状态得到正确的保存和维护。

4. 卸载所有文件系统和设备，并释放所有资源和内存。

5. 重新启动系统并开始执行自检和初始化操作，以确保系统准备好重新启动。

总之，reboot 命令是 Linux 系统重启的标准命令，用于执行系统重启操作并将系统恢复到初始状态。再次提醒，使用 reboot 命令时一定要谨慎，以免对系统造成不良影响。 

## tldr 
 
> 重新启动系统。
> 更多信息：<https://manned.org/reboot.8>.

- 立即重新启动：

`reboot`

- 立即重启，而无需正常关闭：

`reboot -f`