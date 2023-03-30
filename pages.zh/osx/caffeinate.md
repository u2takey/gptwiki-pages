# caffeinate 
## chatgpt 
caffeinate是一个macOS的命令行工具，它可以防止系统进入睡眠模式，可以保持系统的唤醒状态，直到用户使用Ctrl+C，或者手动停止该命令。caffeinate实际上是一个控制系统睡眠的命令行工具，通过向系统内核发送"防止系统睡眠"的信号，从而阻止系统进入节能模式或进入睡眠状态。

caffeinate的语法如下：

```
caffeinate [-dimsu] [-t timeout] [utility [argument ...]]
```

其中，各参数的含义如下：

- -d：防止睡眠、显示关闭以及系统休眠，但仍允许磁盘休眠。
- -i：只防止系统进入睡眠模式。
- -m：防止磁盘休眠。
- -s：防止屏幕保护启动、显示关闭以及系统休眠，但仍允许磁盘休眠。
- -u：防止系统进入睡眠模式，同时防止磁盘休眠。
- -t：指定防止系统睡眠的时间，单位为秒，默认时间为5秒。
- utility [argument ...]：要启动的命令及其参数，即在caffeinate的同时运行其他命令。

例如，运行以下命令将禁止系统进入睡眠状态，同时保持系统唤醒状态30秒钟:

```
caffeinate -i -t 30
```

或者运行以下命令将禁止系统进入睡眠状态，同时运行命令"top"：

```
caffeinate -i top
``` 

## tldr 
 
> 防止 Mac 进入休眠模式。
> 更多信息：<https://ss64.com/osx/caffeinate.html>.

- 防止进入休眠模式 , 1 小时内（3600 秒）：

`caffeinate -u -t {{3600}}`

- 在指定命令执行完前，禁止进入休眠：

`caffeinate -s {{命令}}`

- 在你按 Ctrl-C 之前禁止进入休眠模式：

`caffeinate -i`
