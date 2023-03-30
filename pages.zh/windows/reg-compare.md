# reg compare 
## chatgpt 
reg compare是一个Windows命令行工具，用于比较两个注册表文件的差异。注册表文件是Windows操作系统中存储系统和应用程序设置的重要文件。

该命令有以下语法：

reg compare <RegistryFileName1> <RegistryFileName2>

其中，<RegistryFileName1>和<RegistryFileName2>是两个要比较的注册表文件的文件名（包括完整的路径）。

当执行该命令时，它会比较这两个注册表文件，并返回比较结果的摘要。比较的结果可能会显示：

- 注册表中的每个键及其值的比较结果
- 在一个注册表文件中存在的键，但在另一个文件中不存在的键
- 两个注册表文件的结构差异（例如，一个文件可能包含一个键，而另一个文件可能包含其子键）

此命令还提供了多个选项以更改其行为，例如：

- /a：仅比较值名称、类型和数据，而不比较安全描述符
- /e：仅比较同名键和值，而忽略不同名称的键和值
- /i：在比较时忽略大小写

使用reg compare命令可以帮助系统管理员进行系统维护、故障排除和安全审计。 

## tldr 
 
> 比较注册表中的键和值。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-compare>.

- 比较两个键中的所有值：

`reg compare {{第一个键名}} {{第二个键名}}`

- 比较两个键中指定的值：

`reg compare {{第一个键名}} {{第二个键名}} /v {{值}}`

- 比较两个键中的所有子键和值：

`reg compare {{第一个键名}} {{第二个键名}} /s`

- 仅输出指定键之间匹配的结果：

`reg compare {{第一个键名}} {{第二个键名}} /os`

- 输出两个键之间的匹配和差异：

`reg compare {{第一个键名}} {{第二个键名}} /oa`
