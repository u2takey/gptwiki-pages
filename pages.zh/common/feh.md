# feh 
## chatgpt 
命令：feh

feh 是一个 Linux 下的图像查看器和壁纸设置器，其主要特点包括：

- 可以以终端下显示图像。
- 支持多种图像格式，如 JPEG、PNG 和 GIF 等。
- 可以根据指定的大小，裁剪或缩放图像。
- 可以用作壁纸查看器和设置器，支持自动切换壁纸。
- 可以作为幻灯片播放器，支持设置幻灯片循环和时间间隔等参数。

语法：

feh [参数] [图像文件]

示例：

1. 显示一张图像：

feh /path/to/image.jpg

2. 显示多张图像：

feh /path/to/image1.jpg /path/to/image2.jpg

3. 以幻灯片模式播放多张图像：

feh -z -D 3 /path/to/image1.jpg /path/to/image2.jpg

在上面的示例中，-z 表示循环播放，-D 3 表示每张图像之间的播放时间为 3 秒。

4. 将图像设置为壁纸：

feh --bg-fill /path/to/image.jpg

在上面的示例中，--bg-fill 表示将图像自适应铺满整个屏幕。

5. 显示图像的信息：

feh -l /path/to/image.jpg

在上面的示例中，-l 表示显示图像的信息，如图像的大小、分辨率等。

6. 查看当前目录下所有图片：

feh *.jpg

在上面的示例中，*.jpg 表示查找当前目录下所有以 ".jpg" 结尾的文件。 

## tldr 
 
> 轻量级图像查看工具。
> 更多信息：<https://feh.finalrewind.org>.

- 查看本地图像或使用 URL：

`feh {{图片路径}}`

- 递归查看图像：

`feh --recursive {{图片路径}}`

- 使用无边框窗口查看图像：

`feh --borderless {{图片路径}}`

- 在浏览完最后一个图像之后退出：

`feh --cycle-once {{图片路径}}`

- 设置幻灯片放映周期延迟时间（秒）：

`feh --slideshow-delay {{秒}} {{图片路径}}`

- 设置墙纸（居中、填充、最大化、缩放或平铺）：

`feh --bg-{{center|fill|max|scale|tile}} {{图片路径}}`
