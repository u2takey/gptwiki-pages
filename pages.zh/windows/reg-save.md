# reg save 
## chatgpt 
命令：reg save是用于将指定的注册表键保存到一个文件中的命令。该命令可用于备份和恢复注册表。

语法：reg save KeyName FileName [/y]

参数说明：
- KeyName：必选参数，表示要保存的注册表键的完整路径和名称。例如：HKEY_CURRENT_USER\Software，表示要保存到文件中的是当前用户的“Software”键。
- FileName：必选参数，表示要保存到的文件名（包含路径）。例如：C:\backup\Software.reg，表示要保存到C盘backup文件夹下的Software.reg文件中。如果文件名包含空格，则应该将文件名放在引号内。例如：“C:\backup\My Software.reg”。
- /y：可选参数，表示自动覆盖已存在的同名文件。如果省略该参数，当文件已经存在时，会提示用户是否覆盖。

使用示例：
1. 将HKEY_LOCAL_MACHINE\SOFTWARE中的所有信息保存到C:\backup\Soft.reg文件中：
reg save HKEY_LOCAL_MACHINE\SOFTWARE C:\backup\Soft.reg
2. 将HKEY_CURRENT_CONFIG\SYSTEM键保存到D:\Backup\SystemKey.reg文件中（自动覆盖已存在的文件）：
reg save HKEY_CURRENT_CONFIG\SYSTEM D:\Backup\SystemKey.reg /y 

## tldr 
 
> 将注册表键、子键的所有值保存到一个文件中。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-save>.

- 将注册表键、子键的所有值保存到一个文件中：

`reg save {{键名}} {{文件的路径}}`

- 在没有提示的情况下强制覆盖现有文件：

`reg save {{键名}} {{文件的路径}} /y`
