# fossil-delete 
## chatgpt 
fossil-delete是一个Fossil源码控制系统中的命令，用于删除Fossil仓库中的指定版本或某个文件。

如果不加任何参数，fossil-delete命令会删除最近一次提交的版本，并将此版本从历史记录中移除，但不会真正地将版本从硬盘上删除。如果要彻底删除某个版本，可以使用"--hard"选项。

另外，可以通过指定文件路径的方式删除单个文件或整个目录。例如，"fossil-delete filename"将删除名为"filename"的文件，而"fossil-delete directory"将删除整个名为"directory"的目录。

需要注意的是，一旦一个Fossil版本被删除，就无法再恢复。因此，在执行fossil-delete命令前，应该谨慎考虑并备份重要的版本和文件。 

## tldr 
 
> 这是 `fossil rm` 命令的一个别名。
> 更多信息：<https://fossil-scm.org/home/help/delete>.

- 原命令的文档在：

`tldr fossil rm`
