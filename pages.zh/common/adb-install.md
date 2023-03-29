# adb install 
## chatgpt 
adb install命令是一个用于在Android设备上安装应用程序的adb（Android Debug Bridge）命令。

在执行该命令时，需要先连接Android设备到计算机上，并在设备上启用USB调试。然后在计算机终端中打开adb命令行界面，输入adb install命令，后跟应用程序的.apk文件路径，即可将应用程序安装到设备中。

该命令还支持一些可选的参数，例如“-r”用于替换已经存在的应用程序，而“-s”用于将应用程序安装到设备的外部存储器中。 

## tldr 
 
> 安卓调试桥 -Install: 将应用安装包推送到 Android 模拟器或已连接的安卓设备。
> 更多信息：<https://developer.android.com/studio/command-line/adb>.

- 向模拟器/设备推送安卓 app：

`adb install {{路径/到/应用.apk}}`

- 向特定的模拟器/设备推送安卓 app（覆盖 `$ANDROID_SERIAL`）：

`adb -s {{序列号}} install {{路径/到/应用.apk}}`

- 重装 app, 保持原有数据：

`adb install -r {{路径/到/应用.apk}}`

- 推送一个允许版本代码降级的安卓 app（仅适用于可调试的软件包）：

`adb install -d {{路径/到/应用.apk}}`

- 授予 app manifest 中列举的所有权限许可：

`adb install -g {{路径/到/应用.apk}}`

- 快速部署模式，仅更新 APK 更改过的部分：

`adb install --fastdeploy {{路径/到/应用.apk}}`
