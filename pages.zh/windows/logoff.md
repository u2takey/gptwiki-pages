# logoff 
## chatgpt 
logoff是Windows系统中的一个命令，用于注销当前用户账户。

具体来说，执行logoff命令后，当前用户的所有程序和文件都会被自动保存并关闭，系统会返回登录界面或者锁屏界面，其他用户可以使用自己的账户进行登录。相比于关闭电脑或者重新启动，logoff可以更快捷地切换用户，特别是在共享电脑或者终端服务器上，可以避免其他用户访问当前用户的敏感数据。

Windows系统中可以使用以下方法执行logoff命令：

1. 通过“开始菜单”-“注销”来执行logoff命令；

2. 通过快捷键组合Win+L来锁定屏幕并返回登录界面；

3. 使用命令行工具执行logoff命令，具体命令格式为：logoff [/noconfirm] [/d] [/f] [/p]。其中，/noconfirm表示不进行确认提示，/d表示注销远程连接，/f表示强制注销当前用户，/p表示断开与本地计算机的连接。

需要注意的是，logoff命令只能在管理员权限下执行。同时，当有未保存的文件时，系统会提示用户进行保存操作。 

## tldr 
 
> 注销登录会话。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/logoff>.

- 注销当前会话：

`logoff`

- 通过名称和 id 注销会话：

`logoff {{会话名|会话 id}}`

- 在通过 RDP 连接的特定服务器上注销会话：

`logoff {{会话名|会话 id}} /server:{{服务器名}}`
