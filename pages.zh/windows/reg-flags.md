# reg flags 
## chatgpt 
命令"reg flags"用于显示当前注册表编辑器的标志和状态。该命令会输出一个列表，其中包含了当前注册表编辑器的各种标志和状态的信息。

其中一些常见的标志和状态包括：

- Registry loaded: 表示当前是否已经加载了注册表。
- Hive file loaded: 表示是否已经加载了一个外部的注销表文件。
- Key selected: 表示当前是否已经选择了一个注册表项。
- Value selected: 表示是否已经选择了当前注册表项下的一个值。
- Key created: 表示是否已经创建了一个新的注册表项。
- Value created: 表示是否已经创建了一个新的值，该值将会被添加到当前注册表项下。

除此之外，还有一些其他的标志和状态，它们的具体含义可以参考相关的文档或者使用"reg /?"命令查看帮助信息。 

## tldr 
 
> 显示或设置注册表键的标志。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/reg-flags>.

- 显示当前指定键的标志：

`reg flags {{键名}} query`

- 显示帮助和可用的标志类型：

`reg flags /?`

- 为特定键设置指定以空格分隔的标志，并取消设置未提及的标志：

`reg flags {{键名}} set {{标志 1 标志 2 ..}}`

- 为指定的键和其子键设置标志：

`reg flags {{键名}} set {{标志}} /s`
