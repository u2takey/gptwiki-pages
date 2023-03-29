# at 
## chatgpt 
at 命令用于在指定的时间执行一个命令或脚本，它可以让 Linux 在某个特定的时间执行一些任务，而不需要等待，也不需要手动操作。具体来说，at 命令可以包括两部分内容：指定时间和待执行的任务。

at 命令的使用方法如下：

1.指定时间

可以使用以下格式来指定时间：

```
HH:MM
```
其中，HH 表示小时，MM 表示分钟。例如，要在 14:30 执行某个命令，可以输入以下命令：

```
$ at 14:30
```

2.指定任务

指定任务的方式有几种：

在 at 提示符下输入要执行的命令或脚本。

```
$ at 14:30
at> echo "Hello, World!" > /tmp/hello.txt
at> <EOT>
```
在 at 命令行上使用 `-f` 参数，并指定待执行的脚本文件。

```
$ at 14:30 -f /path/to/script.sh
```

	at 命令还有一些常用的参数，如下：

```
-c              ：取消当前用户下所有至少未开始执行的 at 任务，需跟上任务编号
-l              ：列出当前用户的所有 at 任务
-r              ：使用此参数，可以删除一项 at 任务
-t time         ：使用明确的时间格式指定时间（YYYYMMDDHHMM）
-V              ：输出 at 命令的版本信息
```

使用 `at` 命令时，需要确认 `atd` 服务正在运行，否则 at 命令无法生效。

注意：在 Ubuntu 16.04 LTS、16.10 和 18.04 LTS 版本上测试，如果测试时输入的时间比当前时间晚超过了 24 小时，会返回以下错误提示：

`warning: commands will be executed using /bin/sh
at: the specified time is too far in the future`

这是因为在这些版本的 at 命令默认只能执行 24 小时内的任务。如果想要执行 24 小时之后的任务，可以将相应的配置放在 /etc/at.allow （或 /etc/at.deny）文件中。 

## tldr 
 
> 在指定时间执行命令。
> 更多信息：<https://man.archlinux.org/man/at.1>.

- 打开 `at` 提示符创建一组新的定时命令，按 `Ctrl + D` 保存并退出：

`at {{hh:mm}}`

- 运行命令并通过本地电子邮件程序（例如 sendmail）发送运行结果：

`at {{hh:mm}} -m`

- 在指定时间执行一个脚本：

`at {{hh:mm}} -f {{文件路径}}`

- 在二月十八号下午十一点发送系统通知：

`echo "notify-send '{{Wake up!}}'" | at {{11pm}} {{Feb 18}}`
