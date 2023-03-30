# defaults 
## chatgpt 
defaults命令是一个在Mac OS和iOS操作系统中使用的命令行工具。它用于访问系统和用户默认设置的命令行接口。使用defaults命令可以读取、写入或删除各种默认设置，包括应用程序设置、桌面设置、网络设置、安全设置和其他系统设置。

可用的默认设置可以通过打开终端应用程序，输入defaults命令，然后按下“Tab”键两次，以显示可用的选项列表。其中一些常用的选项包括：

- read：用于读取指定设置的值。
- write：用于设置由键值对表示的特定设置的值。
- delete：用于删除指定的设置。

这些选项后面跟随的参数包括所需的默认设置的路径、键和值。例如，下面是一些示例：

- defaults read com.apple.dock：读取Dock应用程序栏的设置。
- defaults write com.apple.safari “WebKitUserAgent” “MyCustomUserAgent”：将自定义User-Agent添加到Safari浏览器中。
- defaults delete com.apple.finder ShowExternalHardDrivesOnDesktop：删除显示外部硬盘驱动器的Finder桌面设置。

总之，defaults命令是一种十分实用的工具，可以用于修改许多Mac OS和iOS操作系统的默认设置。 

## tldr 
 
> 读取和写入 macOS 应用程序的用户配置。
> 更多信息：<https://ss64.com/osx/defaults.html>.

- 读取应用程序选项的系统默认值：

`defaults read {{应用名}} {{选项}}`

- 读取应用程序选项的默认值：

`defaults read -app {{应用名}} {{选项}}`

- 写入应用程序选项的默认值：

`defaults write {{应用名}} {{选项}} {{- 类型}} {{值}}`

- 加速任务控制界面弹出动画（时间设置为 0.1）：

`defaults write com.apple.Dock expose-animation-duration -float 0.1`

- 删除应用程序的所有默认值：

`defaults delete {{应用名}}`
