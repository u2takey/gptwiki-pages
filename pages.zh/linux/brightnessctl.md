# brightnessctl 
## chatgpt 
brightnessctl 是一个Linux命令行工具，用于调整屏幕亮度。可以使用此命令来增加或减少屏幕的亮度，也可以获取当前亮度级别。

该命令具有以下选项和参数：

选项：
- d：指定显示器的编号
- s：指定屏幕的编号
- m：指定亮度级别的最大值
- M：指定亮度级别的最小值
- p：以百分比输出当前亮度级别

参数：
+：增加亮度
-：减少亮度
设置的亮度级别：值介于最小值和最大值之间的一个整数（例如，0到100之间的数字）

示例用法：

1. 查看当前亮度级别：
brightnessctl
brightnessctl --percentage

2. 将屏幕亮度设置为30％：
brightnessctl set 30

3. 将屏幕亮度增加10％：
brightnessctl set +10

4. 减少屏幕亮度10％：
brightnessctl set -10

5. 查看当前显示器或屏幕的信息：
brightnessctl info 

## tldr 
 
> GUN/Linux 操作系统上用来读取和控制设备亮度的实用工具。
> 更多信息：<https://github.com/Hummer12007/brightnessctl>.

- 列出亮度可变的设备：

`brightnessctl --list`

- 打印显示器当前亮度：

`brightnessctl get`

- 将显示器背光的亮度设置为指定的百分比：

`brightnessctl set {{50%}}`

- 按指定的增量增加亮度：

`brightnessctl set {{+10%}}`

- 将亮度降低指定的递减量：

`brightnessctl set {{10%-}}`
