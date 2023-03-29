# adb shell 
## chatgpt 
adb shell是Android Debug Bridge (ADB)的一个命令，它允许开发者从远程计算机访问安装在Android设备上的命令行界面。它允许你执行一系列命令，与设备进行通信，如：

1.启动Android设备上的Shell：将您连接到Android设备的命令行Shell中。
Shell是一种命令行界面，允许你在设备上执行各种命令。

2.执行命令：在设备的Shell中执行Linux命令或adb命令。

3.运行脚本：可以运行在Android设备上的Shell中执行的脚本。例如，您可以编写并执行一个Shell脚本来设置和配置设备的各种设置。

以下是一些您可以在adb shell中执行的命令示例：

• ls：显示当前目录下的所有文件和文件夹。
• cd：进入到指定的目录。
• mkdir：创建新的目录。
• rm：删除文件或目录。
• cat：查看文件内容。
• ps：显示正在运行的进程。
• su：切换到超级用户（root）模式。
• setprop：设置设备属性值。
• getprop：获取设备属性值。

使用adb shell命令时，您必须先通过USB数据线将Android设备连接到计算机，并启用设备的USB调试功能。这需要您首先在设备的设置中启用开发人员选项，并启用USB调试。 

## tldr 
 
> 安卓调试桥-Shell: 运行安卓模拟器或者连接设备上的远程终端命令。
> 更多信息：<https://developer.android.com/studio/command-line/adb>.

- 启动模拟器/设备上的远程终端：

`adb shell`

- 获取模拟器/设备全部属性：

`adb shell getprop`

- 重置所有运行时权限为它们的默认值：

`adb shell pm reset-permissions`

- 撤销一个应用的危险权限：

`adb shell pm revoke {{包名}} {{权限}}`

- 触发一个键盘敲击事件：

`adb shell input keyevent {{键位码}}`

- 清除模拟器/设备上的数据：

`adb shell pm clear {{包名}}`

- 启动模拟器/设备上的一个行为：

`adb shell am start -n {{包名}}/{{活动名}}`

- 启动模拟器/设备上的首页活动：

`adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN`
