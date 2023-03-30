# rd 
## chatgpt 
rd命令是一个Windows命令行命令，用于删除一个空目录或一个包含空目录的目录树。rd是"remove directory"的缩写，也可以用rmdir命令来执行相同的操作。

语法：rd [drive:] [path] rd [/q] [/s] [drive:]path

参数：
- [drive:] [path] 指定要删除的目录的驱动器位置和路径。
- /q 静默模式，不要提示确认操作。
- /s 删除包含空目录的目录树。

示例：假设当前目录是C:\Users\test，要删除C:\Users\test\mydir目录，可以使用以下命令：rd mydir

注意事项：
- rd命令只能删除空目录或空目录树，如果目录中包含文件或其他子目录，则会出现错误。
- 删除操作是不可逆的，请仔细检查要删除的目录及其路径。
- 如果您尝试删除系统保护的目录，可能会收到访问被拒绝的错误消息，请确保您以管理员身份运行命令提示符。 

## tldr 
 
> 这是 `rmdir` 命令的一个别名。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/rd>.

- 原命令的文档在：

`tldr rmdir`
