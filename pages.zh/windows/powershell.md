# powershell 
## chatgpt 
PowerShell是一种用于管理和自动化Windows操作系统的命令行界面。它提供了一种高级脚本语言和开发工具，用于管理Windows计算机和其他Microsoft产品。

以下是PowerShell的一些主要特点和用途：

1. Powershell能够连接和操作Windows中的各种不同的服务和应用程序，包括文件系统、注册表、远程桌面、IIS、Exchange等等。

2. PowerShell可以使用简洁但强大的命令来自动执行任务，避免手动操作带来的风险和错误。

3. PowerShell提供了丰富的脚本编写功能，支持类、变量、函数、流程控制结构等，使得编写复杂脚本变得更加容易和高效。

4. PowerShell可以通过扩展模块来扩展和提高其功能，例如提供与AWS或Azure等云服务的集成。

总的来说，PowerShell是一个功能强大而灵活的工具，可以帮助Windows管理员和开发人员快速自动化和进行系统管理任务，提高效率和准确性。 

## tldr 
 
> 专为系统管理而设计的命令行 shell 和脚本语言。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/powershell>.

- 在命令提示符窗口中启动 Windows PowerShell 会话：

`powershell`

- 加载一个特定的 PowerShell 控制台文件：

`powershell -PSConsoleFile {{路径/file}}`

- 用指定版本的 PowerShell 启动会话：

`powershell -Version {{版本}}`

- 防止运行启动命令后 shell 退出：

`powershell -NoExit`

- 描述发送到 PowerShell 的数据格式：

`powershell -InputFormat {{Text|XML}}`

- 设定 PowerShell 输出的格式：

`powershell -OutputFormat {{Text|XML}}`

- 显示帮助：

`powershell -Help`
