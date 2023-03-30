# reg unload 
## chatgpt 
"reg unload"是一条Windows注册表命令，用于从系统中卸载一个以前加载的注册表文件。

当用户或系统管理员运行"reg load"命令时，注册表文件将被加载到系统中，提供对存储在其中的键和值的访问。一旦完成对注册表文件的访问，用户或管理员可以使用"reg unload"命令将其卸载，以释放系统资源并保护注册表的完整性。

使用"reg unload"命令时，需要指定已加载注册表文件的路径。例如，以下命令将卸载名为"MyRegistry"的注册表文件：

reg unload HKLM\MyRegistry

请注意，必须以管理员身份运行"reg unload"命令以卸载注册表文件。如果未以管理员身份运行该命令，则会返回"访问被拒绝"错误。 

## tldr 
 
> 从使用`reg load`命令加载的注册表中删除数据。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-unload>.

- 从使用`reg load`命令加载的注册表中删除数据：

`reg unload {{键名}}`
