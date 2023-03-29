# flameshot 
## chatgpt 
flameshot是一个开源的截图和注释工具，用于Linux操作系统。它可以帮助用户轻松地截取屏幕上的任何部分，并提供一系列丰富的注释工具，例如箭头、矩形、圆形、线条和文字等。flameshot还可以让用户在截图完成后进行编辑和保存。

flameshot常用的命令包括：

1. flameshot gui：启动flameshot的GUI界面，用户可以从菜单中选择截图模式，并使用注释工具编辑截图。

2. flameshot full：截取整个屏幕。

3. flameshot screen：选择截图区域。

4. flameshot select：矩形截图模式，用户可以使用鼠标在屏幕上选择任意矩形区域进行截图。

5. flameshot launch：使用默认设置启动flameshot。

6. flameshot config：打开flameshot的配置文件，用户可以根据自己的需求进行修改和设置。

总之，flameshot是一款功能强大且易于使用的截图和注释工具，可以大大提高Linux用户的工作效率。 

## tldr 
 
> 带有 GUI 界面的 Screenshot 工具。
> 支持基本的图像编辑，例如文本，形状，颜色和 imgur。
> 更多信息：<https://flameshot.org>.

- 全屏截图：

`flameshot full`

- 交互式截图：

`flameshot gui`

- 截图并保存到特定的路径：

`flameshot gui --path {{路径/到/目录}}`

- 简单模式下交互式截图：

`flameshot launcher`

- 指定屏幕截图：

`flameshot screen --number {{2}}`

- 截图并打印到标准输出：

`flameshot gui --raw`

- 截图并复制到剪切板：

`flameshot gui --clipboard`

- 延迟指定毫秒时间截图：

`flameshot full --delay {{5000}}`
