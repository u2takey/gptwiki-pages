# eventcreate 
## chatgpt 
eventcreate是Windows操作系统中的一个命令行工具，可以创建自定义事件日志。它提供了一种创建自定义事件并将其记录到本地或远程计算机的日志文件中的方法。以下是一些可用的选项和参数：

- /t：事件类型。可以是成功、错误或警告。
- /id：事件ID。应该是一个整数值。
- /l：事件日志。应该是一个有效的事件日志名称。
- /so：源。应该是事件源名称。
- /d：事件说明。可以是一个字符串值。

例如，要在“应用程序”事件日志中创建一个具有ID 1000、源名称“MyApp”和类型“成功”的事件，说明为“MyApp运行成功”，可以使用以下命令：

eventcreate /t SUCCESS /id 1000 /l APPLICATION /so MyApp /d "MyApp运行成功"

执行该命令将创建一个新的事件并将其记录到应用程序事件日志中。在事件查看器中可以查看该事件。 

## tldr 
 
> 在事件日志中创建自定义条目。
> 事件 ID 可以是 1 到 1000 之间的任意数值。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/eventcreate>.

- 在日志中创建一个具有给定 id（1-1000）的新事件：

`eventcreate /t {{success|error|warning|information}} /id {{id}} /d "{{消息}}"`

- 在特定事件日志中创建事件：

`eventcreate /l {{日志名}} /t {{类型}} /id {{id}} /d "{{消息}}"`

- 为新创建的事件指定来源：

`eventcreate /so {{来源名}} /t {{类型}} /id {{id}} /d "{{消息}}"`

- 在远程计算机的事件日志中创建事件：

`eventcreate /s {{主机名}} /u {{用户名}} /p {{密码}} /t {{类型}} /id {{id}} /d "{{消息}}"`
