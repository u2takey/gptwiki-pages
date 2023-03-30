# reg restore 
## chatgpt 
命令reg restore是一个Windows命令行工具，用于还原或恢复指定的注册表文件。

该命令的语法格式如下：

```reg restore <Key> <FileName>```

其中，Key是注册表中的键路径，FileName是要还原的注册表文件名及路径。

例如，如果要将注册表文件mybackup.reg还原到键路径HKEY_CURRENT_USER\Software\MyApp中，可以使用以下命令：

```reg restore HKEY_CURRENT_USER\Software\MyApp mybackup.reg```

需要注意的是，使用reg restore命令需要以管理员身份运行命令提示符。 

## tldr 
 
> 从备份文件中恢复键和值。
> 参见 `reg-save` 来获取更多的信息。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-restore>.

- 使用备份文件中的数据覆盖指定的键：

`reg restore {{键名}} {{文件路径}}`
