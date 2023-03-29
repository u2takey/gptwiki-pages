# write 
## chatgpt 
命令 write 用于向已登录系统的用户发送消息或者允许其他用户向终端发送消息。使用 write 命令需要指定目标用户的用户名和要发送的消息，消息发送后将在目标用户的终端上显示。

语法：

write [用户名] [终端]

参数说明：

- 用户名：指定目标用户的用户名。
- 终端：指定要发送消息的终端。

使用示例：

1. 向指定用户发送消息：

```
write alice
Hello Alice, how are you?
```

2. 指定终端发送消息：

```
write tty1
What are you working on?
```

注意事项：

- 发送消息的用户需要具有向目标用户终端发送消息的权限。
- 目标用户必须已登录系统并打开了终端。
- 发送的消息内容中不能包含特殊字符，如 $、%、# 等。
- 如果未指定终端，则默认发送到当前用户正在使用的终端。 

## tldr 
 
> 向某个终端上的特定用户的屏幕写入信息（Ctrl-C 来停止写入）。
> 使用 `who` 命令来获取所有活动用户的终端 id. 参见 `mesg`.
> 更多信息：<https://manned.org/write>.

- 向指定的终端 ID 上的指定用户写入信息：

`write {{username}} {{terminal_id}}`

- 向终端 "/dev/tty/5" 上的用户 "testuser" 发送信息：

`write {{testuser}} {{tty/5}}`

- 向伪终端 "/dev/pts/5" 上的用户 "johndoe" 发送信息：

`write {{johndoe}} {{pts/5}}`
