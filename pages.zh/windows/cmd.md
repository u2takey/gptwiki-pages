# cmd 
## chatgpt 
cmd是Windows操作系统中一个命令行解释器，它允许用户在命令行中执行各种操作和指令。以下是一些常见的cmd命令和其作用：

1. dir：列出当前目录下的文件和子目录。
2. cd：进入指定目录。
3. mkdir：创建一个新目录。
4. del：删除文件。
5. copy：复制文件或目录。
6. type：显示一个文本文件的内容。
7. ping：测试与其他计算机的连接。
8. ipconfig：查看网络配置信息。
9. netstat：显示计算机与网络之间的活动连接。
10. tasklist：显示正在运行的进程列表。
11. shutdown：关闭计算机。
12. help：显示帮助文档。

这些命令可以用于管理文件、网络、系统进程等方面的操作。 

## tldr 
 
> Windows 命令解释器。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/cmd>.

- 开启一个新的命令行实例：

`cmd`

- 运行指定的命令然后退出：

`cmd /c "{{命令}}"`

- 执行一个指定的命令，之后进入一个交互式 shell：

`cmd /k "{{命令}}"`

- 不显示命令的输出结果：

`cmd /q`

- 启用或禁用命令扩展：

`cmd /e:{{on|off}}`

- 启用或禁用文件和目录名的自动补全：

`cmd /f:{{on|off}}`

- 启用或禁用环境变量扩展：

`cmd /v:{{on|off}}`

- 强制输出内容使用 Unicode 编码：

`cmd /u`
