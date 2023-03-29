# adb reverse 
## chatgpt 
adb reverse命令是Android Debug Bridge工具的一个命令，它可以将设备上的某个端口(例如：设备上的80端口)映射到本地开发机器上的另一个端口(例如：本地机器上的8080端口)。这个命令通常用于在本地环境中进行开发和测试，因为它允许您在不离开本地环境的情况下访问设备上的服务。

具体来说，adb reverse命令有以下用处:
1. 将设备上的端口映射到本地开发机器上的对应端口，方便本地开发和测试；
2. 提供调试网络连接的受控环境，以确保应用程序可以将请求正确地发送到另一个端口；
3. 允许您访问设备上的某些服务，例如Android模拟器中运行的本地主机上的服务。

使用adb reverse命令，您可以执行以下操作:
1. 映射设备上的某个端口到本地机器上的另一个端口;
2. 反向映射本地机器上的某个端口到设备上的另一个端口;
3. 列出当前映射的端口。

用法示例:
1. 将远程设备80端口映射到本地8080端口: adb reverse tcp:8080 tcp:80
2. 反向映射本地机器上的8080端口到设备上的80端口: adb reverse tcp:80 tcp:8080
3. 列出当前映射的端口: adb reverse --list

需要注意的是，使用adb reverse命令时需要确保Android设备已经连接到开发机，并开启了adb调试模式。 

## tldr 
 
> 安卓调试桥-反射： 反向映射安卓模拟器实例或者已连接的实体设备的套接字连接。
> 更多信息：<https://developer.android.com/studio/command-line/adb>.

- 列出所有来自模拟器和设备的映射连接：

`adb reverse --list`

- 将 TCP 端口从安卓模拟器或设备中映射到 localhost：

`adb reverse tcp:{{远程端口}} tcp:{{本地端口}}`

- 从安卓模拟器或设备移除一个反向 socket 连接：

`adb reverse --remove tcp:{{远程端口}}`

- 从安卓模拟器或设备移除所有反向 socket 连接：

`adb reverse --remove-all`
