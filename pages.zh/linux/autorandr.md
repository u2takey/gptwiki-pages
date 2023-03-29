# autorandr 
## chatgpt 
Autorandr是一个Linux命令行工具，用于自动检测和配置连接到计算机的显示器。它可以根据不同的设置情况来自动切换分辨率、旋转方向、输出设置等。

使用autorandr，用户可以轻松地保存和切换不同的显示器配置，例如在办公室和家庭使用不同的显示器或连接到项目根据需要自动更改显示器设置。

此外，autorandr还具有支持外部脚本和自定义配置文件的功能，以便根据用户需要自定义显示器配置。

下面是示例命令：

- autorandr -l ：列出当前所有可用的显示器配置。
- autorandr --save work：保存当前的显示器配置为名称work。
- autorandr --change work：切换到名称为work的显示器配置。
- autorandr -r：重新加载显示器设置。 

总之，Autorandr使得在Linux系统中自动配置和管理多个显示器变得更加简单和方便。 

## tldr 
 
> 自动调节屏幕布局。
> 更多信息：<https://github.com/phillipberndt/autorandr>.

- 保存当前屏幕布局：

`autorandr -s {{配置文件名}}`

- 显示保存的配置：

`autorandr`

- 切换设置：

`autorandr -l {{配置文件名}}`

- 设置默认设置：

`autorandr -d {{配置文件名}}`
