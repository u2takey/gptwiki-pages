# shutdown 
## chatgpt 
shutdown是一个操作系统命令，用于让计算机关闭、重新启动或者进入睡眠状态。

常用的命令参数有：

- -s：用于关闭计算机
- -r：用于重新启动计算机
- -h：用于进入睡眠状态
- -t：指定时间（单位为秒）后执行命令。例如，“shutdown -s -t 3600”表示在3600秒后关闭计算机。

其中，-s和-r需要管理员权限才能使用。

在Windows操作系统中，可以在“命令提示符”或者“运行”中输入shutdown命令来执行。在Linux或者Unix操作系统中，可以在终端或者控制台中输入该命令来执行。 

## tldr 
 
> 用于关闭，重新启动或注销计算机的工具。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/shutdown>.

- 关闭当前的计算机：

`shutdown /s`

- 重启当前的计算机：

`shutdown /r`

- 休眠当前的计算机：

`shutdown /h`

- 注销当前的计算机：

`shutdown /l`

- 指定在关闭之前等待的时间（以秒为单位）：

`shutdown /s /t {{秒}}`

- 指定一个关机的理由：

`shutdown /s /c "{{理由}}"`

- 在超时之前取消关机指令：

`shutdown /a`

- 关闭远程的计算机：

`shutdown /m {{\\ 主机名}}`
