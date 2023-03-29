# betterlockscreen 
## chatgpt 
betterlockscreen 命令是用于自定义 Linux 操作系统的锁屏屏幕的工具。它可以提供各种选项来设计锁屏屏幕，如背景图像、字体样式、时间格式、随机图片等。这些选项可以通过配置文件进行设置，并且全局的配置文件在 /etc/betterlockscreenrc 目录下，每个用户的个人配置文件则存储在 $HOME/.config/betterlockscreen 目录中。

要在系统中使用 betterlockscreen 命令，需要通过包管理器安装 betterlockscreen 工具，通常可以使用以下命令进行安装：

```sudo apt-get install betterlockscreen```

安装完成后，可以通过以下命令来使用 betterlockscreen：

```betterlockscreen -u /path/to/background/image```

以上命令将使用指定的图片作为锁屏背景。除此之外，还可以使用其他选项来自定义锁屏屏幕。例如：

```betterlockscreen -u /path/to/background/image -t "My Lock Screen" -r 1920x1080```

这个命令将使用指定的图片，并在锁屏屏幕上显示自定义的标题（即“My Lock Screen”）。同时，锁屏屏幕的分辨率将设置为 1920x1080。

总之，betterlockscreen 命令提供了许多选项来自定义 Linux 操作系统的锁屏屏幕，使用户可以轻松地使其个性化和更美观。 

## tldr 
 
> 简洁的锁屏程序。
> 更多信息：<https://github.com/pavanjadhaw/betterlockscreen>.

- 锁定屏幕：

`betterlockscreen --lock`

- 更换锁屏背景：

`betterlockscreen -u {{图片.png}}`

- 锁屏并显示一些自定义文本：

`betterlockscreen -l pixel -t "{{自定义锁屏文本}}"`

- 锁屏并自定义显示屏关闭超时秒数：

`betterlockscreen --off {{5}} -l`
