# reg export 
## chatgpt 
reg export是一个Windows命令行工具，用于将Windows注册表中的一个或多个键值导出到一个文件中。它的语法如下：

reg export <键名> <文件名> [/y]

其中：<键名>指定要导出的键或子键的名称，可以使用完整路径或仅限于子键的名称；<文件名>指定生成的文件名，可以使用任何有效路径；/y选项指定在存在目标文件时覆盖它。

当成功执行时，reg export会将指定键或子键以及其所有子项和值导出到指定文件中。导出的文件包含可以使用REGEDIT.exe或reg import命令导入回注册表的信息。

以下是使用reg export的示例：

1. 导出“HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion”键到名为“regbackup.reg”的文件中：

reg export HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion regbackup.reg

2. 导出“HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Run”子键到名为“startup.reg”的文件中：

reg export HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Run startup.reg

通过使用reg export命令，用户可以轻松地备份和还原他们的注册表设置，更改系统配置，并在需要时恢复到以前的状态。 

## tldr 
 
> 将指定的子键和值导出到文件中。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-export>.

- 导出指定键下所有的子键和值：

`reg export {{键名}} {{导出文件的路径.reg}}`

- 在没有提示的情况下强制覆盖现有文件：

`reg export {{键名}} {{导出文件的路径.reg}} /y`
