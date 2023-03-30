# fondue 
## chatgpt 
fondue是一种瑞士菜品，通常由芝士和白葡萄酒混合在一起融化，并且可以在火上蘸面包、蔬菜、水果等食物。在计算机领域，fondue是一种用于汇集和显示系统性能和统计信息的工具。它可以提供有关内存使用情况、CPU使用情况、网络流量等信息，帮助管理员了解系统的运行状态和性能瓶颈，并作出相应的优化和改进。

在命令行界面中，fondue是一个在Windows操作系统中使用的命令，用于在一个已安装的.NET Framework版本中列出所有文件和文件夹。该命令的语法如下：
```
fondue [/? | /v[:<Level>] [/s[:<State>]] [/nologo] <Assembly> [<Assembly> [...]]]
```
其中，各参数的含义如下：
- /?：显示帮助信息。
- /v：指定详细等级，Level的取值范围为0-4，默认值为2。
- /s：指定程序集的状态，State的取值范围为0-3，默认值为3。
- /nologo：禁用显示启动标语。
- Assembly：要显示信息的程序集的名称。

使用fondue命令可以显示有关已安装.NET Framework版本中程序集依赖关系和文件信息。这对识别应用程序运行时可能发生的问题非常有用，可以帮助管理员快速定位问题并采取适当的措施。 

## tldr 
 
> 可选 Windows 功能的命令行安装程序。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/fondue>.

- 启用一个指定的 Windows 功能：

`fondue /enable-feature:{{功能}}`

- 向用户隐藏所有输出信息：

`fondue /enable-feature:{{功能}} /hide-ux:all`

- 为错误报告指定调用者进程名称：

`fondue /enable-feature:{{功能}} /caller-name:{{名称}}`
