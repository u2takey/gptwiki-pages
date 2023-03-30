# driverquery 
## chatgpt 
driverquery是一个Windows命令行工具，它用于列出当前系统上安装的驱动程序列表。它可以显示每个驱动程序的名称、类型、描述、公司名、版本号和日期。

使用driverquery命令，您可以了解有关正在运行的系统驱动程序的更多信息，这对于调试系统问题或检查系统安全性非常有用。

以下是driverquery命令的基本用法：

driverquery [/fo format] [/nh] [/v] [/si] [/qu path] [/group OrderBy]
/fo format - 指定输出格式（表格、列表或CSV格式）
/nh - 不包括列标题
/v - 显示详细信息，包括驱动程序的数字签名、状态、启动类型和路径
/si - 显示驱动程序签名信息
/qu path - 仅列出指定路径下的驱动程序（例如，driverquery /qu C:\Windows\System32\drivers）
/group OrderBy - 按指定的顺序组合显示驱动程序列表（例如，driverquery /group Company）

例如，如果您要列出系统上所有驱动程序的基本信息，可以使用以下命令：

driverquery

如果要查看更详细的信息以及数字签名和启动类型，请使用以下命令：

driverquery /v

如果要按公司名组织驱动程序列表，请使用以下命令：

driverquery /group Company 

## tldr 
 
> 显示已安装设备驱动程序的信息。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/driverquery>.

- 显示所有已安装设备驱动程序的列表：

`driverquery`

- 以指定格式显示驱动程序的列表：

`driverquery /fo {{table|list|csv}}`

- 显示带有列的驱动程序列表，以表明它们是否已签名：

`driverquery /si`

- 排除输出列表中的标题：

`driverquery /nh`

- 显示远程计算机的驱动程序列表：

`driverquery /s {{主机名}} /u {{用户名}} /p {{密码}}`

- 显示详细信息的驱动程序列表：

`driverquery /v`

- 显示详细的使用信息：

`driverquery /?`
