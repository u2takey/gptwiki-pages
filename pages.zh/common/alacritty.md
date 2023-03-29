# alacritty 
## chatgpt 
alacritty是一个跨平台的，GPU加速的终端仿真器，使用Rust编写，旨在提供更快，更易于使用的终端应用程序。

当运行该命令时，将启动alacritty终端窗口，用户可以在其中与其它终端应用程序一样运行各种命令和程序。默认情况下，alacritty只显示一个简单的黑色背景和白色的文本，但是它具有许多可配置的选项，用户可以根据自己的偏好进行自定义设计。

可以在alacritty中使用的一些常用快捷键，包括：

1. Ctrl + Shift + C 复制选中的文本
2. Ctrl + Shift + V 粘贴文本
3. Ctrl + Shift + T 新建一个选项卡
4. Ctrl + Shift + W 关闭当前选项卡

总的来说，alacritty是一个轻量级，高度可定制和快速运行的终端应用程序，适合开发人员、Linux用户和其他需要频繁使用终端的人员使用。 

## tldr 
 
> 跨平台，GPU 加速的终端模拟器。
> 更多信息：<https://github.com/alacritty/alacritty>.

- 打开一个新的 Alacritty 窗口：

`alacritty`

- 运行在指定目录中：

`alacritty --working-directory {{路径}}`

- 在新的 Alacritty 窗口中运行命令：

`alacritty -e {{命令}}`

- 指定备用配置文件（默认在 `$XDG_CONFIG_HOME/alacritty/alacritty.yml`）：

`alacritty --config-file {{路径/config.yml}}`

- 在启用实时配置重新加载的情况下运行（默认情况下也可以在 `alacritty.yml` 中启用）：

`alacritty --live-config-reload --config-file {{路径/config.yml}}`
