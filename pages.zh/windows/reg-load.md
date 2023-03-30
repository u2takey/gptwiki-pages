# reg load 
## chatgpt 
命令：reg load是Windows中的一个注册表命令，用于在当前计算机上加载另一个计算机的注册表。

具体来说，reg load命令的语法如下：

> reg load HKLM\TempHive <FileName>

其中，HKLM\TempHive表示要加载的注册表键路径，<FileName>表示要加载的注册表文件路径。

例如，如果要在当前计算机上加载另一个计算机上的HKEY_LOCAL_MACHINE\SYSTEM键，可以使用以下命令：

> reg load HKLM\TempHive C:\Users\UserName\Desktop\SYSTEM

这将会把C:\Users\UserName\Desktop\SYSTEM文件中的注册表数据加载到当前计算机的HKLM\TempHive键中。

需要注意的是，使用reg load命令需要具有管理员权限。此外，加载的注册表数据只在当前会话中有效，即在命令行窗口关闭后数据将会被卸载。如果需要长期使用，可以使用reg save命令将加载的数据保存到注册表文件中。 

## tldr 
 
> 将保存的子键加载到不同的子键中。
> This is intended for troubleshooting and temporary keys.
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-load>.

- 将备份文件加载到指定的键中：

`reg load {{键名}} {{文件的路径}}`
