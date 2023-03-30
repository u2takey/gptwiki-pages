# msg 
## chatgpt 
msg命令是Windows系统中的一个命令行程序，主要功能是向指定的用户或计算机发送消息。

使用该命令时，需要指定接收消息的用户或计算机名称，以及要发送的消息内容。

例如，向计算机名为"COMPUTER001"的用户"User1"发送消息"Hello, World!"的命令为：

```
msg User1 /SERVER:COMPUTER001 "Hello, World!"
```

其中，"/SERVER"参数指定要向哪个计算机发送消息，"User1"为接收消息的用户名，"Hello, World!"为要发送的消息内容。

需要注意的是，使用msg命令发送消息时，必须保证接收消息的计算机启用了"消息服务"功能，否则发送消息将失败。

另外，该命令也可以用于向远程计算机发送消息，只需在"/SERVER"参数中指定远程计算机的名称或IP地址即可。 

## tldr 
 
> 向指定的用户或会话发送信息。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/msg>.

- 向指定的用户或会话发送信息：

`msg {{用户名|会话名|会话 id}} {{信息}}`

- 从标准输入发送信息：

`echo "{{信息}}" | msg {{用户名|会话名|会话 id}}`

- 向指定的服务器发送消息：

`msg /server:{{服务器名称}} {{用户名|会话名|会话 id}}`

- 向当前计算机的所有用户发送消息：

`msg *`

- 设置发送消息的延迟：

`msg /time:{{秒}}`
