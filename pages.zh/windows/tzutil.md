# tzutil 
## chatgpt 
tzutil是Windows操作系统中的命令行工具，用于管理和更改时区设置。

具体命令及其功能如下：

1. tzutil /g ：查询当前系统的时区设置信息，包括时区名称、偏移量（UTC +/-几个小时）和当前时区所使用的夏令时规则。

2. tzutil /l ：列出所有可用的时区列表。该命令将在命令行窗口中显示一个新的列表，其中包含所有可用的时区名称。

3. tzutil /s [时区名称] ：更改系统的时区设置。需要将时区名称作为参数传递给该命令，例如：tzutil /s "China Standard Time"。注意，必须使用双引号将时区名称括起来，否则该命令可能无法正常工作。

4. tzutil /? ：显示tzutil命令的帮助信息。

通过使用tzutil命令，用户可以轻松管理和更改时区设置，以确保机器显示正确的本地时间。此外，tzutil命令还可以与其他系统管理工具结合使用，例如批处理文件或PowerShell脚本，以便快速自动化系统设置。 

## tldr 
 
> 用于显示或配置系统时区的工具。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/tzutil>.

- 获取当前的时区：

`tzutil /g`

- 显示可用的时区列表：

`tzutil /l`

- 将系统时区设置为特定值：

`tzutil /s {{时区 id}}`
