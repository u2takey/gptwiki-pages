# wacaw 
## chatgpt 
wacaw是一款命令行工具，用于在Linux系统中捕获照片和视频。该工具可以从系统内置摄像头或外部摄像头捕获图像和视频，并可以设置各种参数，如图像质量、分辨率、帧数等。

具体使用方式如下：

安装wacaw：

在Ubuntu或Debian上使用以下命令安装：

sudo apt-get install wacaw

捕获图像：

要捕获一张图像，请使用以下命令：

wacaw -p filename.jpg

其中，"-p"参数指定要捕获的图像。 filename.jpg是指定的要保存的文件名。 

捕获视频：

要捕获视频，请使用以下命令：

wacaw -v filename.avi

其中，"-v"参数指定要捕获的视频。 filename.avi是指定的要保存的文件名。

设置参数：

可以使用不同的参数设置捕获图像或视频的质量、分辨率、帧数等。以下是一些例子：

捕获分辨率为640x480的图像：

wacaw -p filename.jpg -r 640x480

捕获分辨率为640x480、帧率为30的视频：

wacaw -v filename.avi -r 640x480 -f 30

捕获高质量图像：

wacaw -p filename.jpg -q 95

以上就是关于wacaw命令的详细解释。 

## tldr 
 
> 一个用于 macOS 的小命令行工具，允许您从连接的摄像头捕获静止图片和视频。
> 更多信息：<http://webcam-tools.sourceforge.net>.

- 从网络摄像机拍照：

`wacaw {{文件名}}`

- 录制视频：

`wacaw --video {{文件名}} -D {{录制多少秒}}`

- 用自定义分辨率拍照：

`wacaw -x {{宽}} -y {{高}} {{文件名}}`

- 将刚拍摄的图像复制到剪贴板：

`wacaw --to-clipboard`

- 可用设备列表：

`wacaw -L`
