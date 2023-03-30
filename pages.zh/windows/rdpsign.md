# rdpsign 
## chatgpt 
rdpsign是一个Windows操作系统中命令行工具，用于数字签名远程桌面连接(RDP)文件。该命令可用于保护RDP文件，以确保只有授权用户才能连接到远程计算机。

具体来说，使用rdpsign命令进行数字签名，可以将一个有效的数字证书与RDP文件相关联。此数字证书将确保远程桌面连接是安全的，并且只有经过身份验证和授权的用户才能访问。

以下是rdpsign命令的基本语法：

rdpsign /sha1 <Thumbprint> /q <Path to RDP file>

其中，/sha1选项指定要使用的数字证书的指纹(Thumbprint)，/q选项指定要签名的RDP文件的路径。

需要注意的是，使用rdpsign命令进行数字签名需要有管理员权限，否则将无法签名成功。此外，必须先在本地计算机上安装有效的数字证书才能进行数字签名。 

## tldr 
 
> 用于签名远程桌面协议（RDP）文件的工具。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/rdpsign>.

- 为一个 RDP 文件签名：

`rdpsign {{文件路径.rdp}}`

- 使用一个指定的 sha256 哈希值为 RDP 文件签名：

`rdpsign {{文件路径.rdp}} /sha265 {{哈希值}}`

- 启用静默输出：

`rdpsign {{文件路径.rdp}} /q`

- 显示详细的信息、警告和状态：

`rdpsign {{文件路径.rdp}} /v`

- 在不更新文件的情况下将输出显示到标准输出来测试签名：

`rdpsign {{文件路径.rdp}} /l`
