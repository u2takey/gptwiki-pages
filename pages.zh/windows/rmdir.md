# rmdir 
## chatgpt 
rmdir命令是一个用于删除指定目录的命令。rmdir表示remove directory（删除目录），该命令会删除空目录，即目录中没有任何文件或子目录。

使用rmdir命令的语法如下所示：

rmdir [选项] 目录名

选项说明：

- -p：如果父目录也是空的，将其删除。
- -v：详细显示命令执行过程。

需要注意的是，如果目录中还有文件或子目录，使用该命令将会失败并显示一个错误消息。

实例：

假设我们有一个目录"test"，我们可以使用以下命令删除它：

rmdir test

如果该目录下存在文件或子目录，我们应该首先删除它们，然后再使用rmdir命令删除该目录。如果想删除目录及其子目录和文件，应该使用rm -rf命令。 

## tldr 
 
> 删除一个目录和其中的内容。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/rmdir>.

- 删除一个空目录：

`rmdir {{目录的路径}}`

- 递归删除一个目录及其中的内容：

`rmdir {{目录的路径}} /s`

- 在没有提示的情况下递归删除目录及其内容：

`rmdir {{path/to/directory}} /s /q`
