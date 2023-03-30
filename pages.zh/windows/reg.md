# reg 
## chatgpt 
reg命令是Windows操作系统中的注册表编辑器命令行工具，用于在命令行界面下对Windows注册表进行查看、修改、导入、导出等操作。 

以下是reg命令的常见用法：

1. reg query：查询注册表的指定键值，并将结果输出到控制台窗口。

2. reg add：添加一个新的注册表项、键值和数据

3. reg delete：删除一个注册表项、键值和数据

4. reg export：将指定的注册表键导出到指定的文件

5. reg import：将指定文件中存储的注册表键值导入到Windows注册表中

6. reg save：将指定的注册表键保存到指定的文件中

7. reg restore：将指定的注册表备份文件还原到Windows注册表中。

reg命令可以在安装Windows操作系统的系统上直接使用，无需安装额外的软件。它可以帮助用户快速地对Windows注册表进行操作，并且可以在脚本中自动化处理注册表操作。 

## tldr 
 
> 用于在 Windows 注册表中管理键及其值的命令行界面。
> 此命令也有关于其子命令的文件，例如：`reg add`.
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg>.

- 执行注册表命令：

`reg {{命令}}`

- 显示常规信息并列出所有可用命令：

`reg /?`

- 显示指定命令的帮助信息：

`reg {{命令}} /?`
