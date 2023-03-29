# adb 
## chatgpt 
adb（Android Debug Bridge）是一个 Android 开发工具，用于在计算机和 Android 设备之间进行通信。它允许开发人员在命令行上执行各种操作，包括在设备上安装和调试应用程序，访问设备文件系统，复制文件到和从设备，以及发送命令到设备执行。以下是一些常见的 adb 命令：

1. adb devices：列出连接到计算机的所有设备。

2. adb shell：打开与设备的命令行交互界面。

3. adb push <local> <remote>：将本地文件复制到设备上。

4. adb pull <remote> <local>：将设备上的文件复制到本地。

5. adb install <path>/<appname>.apk：安装设备上的 APK 文件。

6. adb uninstall <package-name>：从设备中卸载应用程序。

7. adb logcat：显示设备上的日志信息。

8. adb reboot：重新启动设备。

9. adb shell dumpsys <service>：显示设备服务的信息。

10. adb forward <tcp> <device>：将 TCP 端口从设备转发到主机。 

## tldr 
 
> 安卓调试桥：与 Android 模拟器或已连接的 Android 设备通信。
> 此命令也有关于其子命令的文件，例如：`adb shell`.
> 更多信息：<https://developer.android.com/studio/command-line/adb>.

- 检查 adb server 进程的是否在运行，并开启它：

`adb start-server`

- 终止 adb server 进程：

`adb kill-server`

- 在目标模拟器 / 设备实例上开启一个远程 shell：

`adb shell`

- 将 Android 应用程序推送到模拟器 / 设备：

`adb install -r {{路径/到/应用.apk}}`

- 从目标设备上拷贝一个文件 / 目录到本地：

`adb pull {{路径/到/设备的文件或目录}} {{路径/到/本地上的目录}}`

- 从本地拷贝一个文件 / 目录到目标设备：

`adb push {{路径/到/本地文件或目录}} {{路径/到/设备上的目录}}`

- 列出已连接的设备：

`adb devices`
