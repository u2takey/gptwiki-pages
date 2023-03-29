# airmon-ng 
## chatgpt 
airmon-ng 是一个 Linux 环境下的无线网络监控工具，用于监听无线网络接口。它是在 Aircrack-ng 工具套装中的一个组件，主要被用来监控 Wi-Fi 网络以实现网络安全措施。

使用 airmon-ng，可以实现以下任务：

1. 监听某个无线网络接口的无线活动；
2. 显示当前所有的无线接口；
3. 让无线接口进入监听模式，并显示有哪些进程在使用这个接口；
4. 扫描无线网络，以获取SSID（服务集标识符）、BSSID（基础设施标识符）和信道信息等。

具体的命令选项如下：

1. airmon-ng start [interface]：将接口设置为监听模式；
2. airmon-ng stop [interface]：停止接口的监听模式；
3. airmon-ng check [interface]：检查接口是否可以使用airmon-ng；
4. airmon-ng status：显示当前所有无线接口的情况；
5. airmon-ng check kill：强制停止所有无线接口的进程并释放资源；
6. airmon-ng start [interface] [channel]：使用指定的无线通道启动监听模式；
7. airmon-ng start [interface] [channel] [band]：使用指定的无线通道和无线带宽启动监听模式；
8. airmon-ng stop [monitor interface]：停止指定的监听模式。

总之，airmon-ng 是一款有用的无线网络监控工具，可以在网络安全测试、调试等方面提供极大的帮助。 

## tldr 
 
> 激活无线网络设备的监控模式。
> 更多信息：<https://www.aircrack-ng.org/doku.php?id=airmon-ng>.

- 列出无线设备和它们的状态：

`sudo airmon-ng`

- 为一个特定的设备打开监控模式：

`sudo airmon-ng start {{wlan0}}`

- 关闭使用无线设备的干扰进程：

`sudo airmon-ng check kill`

- 关闭某个特定网络接口的监控模式：

`sudo airmon-ng stop {{wlan0mon}}`
