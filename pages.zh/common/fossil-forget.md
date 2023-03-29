# fossil-forget 
## chatgpt 
fossil-forget是Fossil版本控制系统中的一个命令，用于将一个或多个文件或目录从版本控制系统中删除，不再跟踪它们的更改历史。

使用fossil-forget命令后，文件或目录将从版本控制系统中消失，但不会从磁盘上删除。这意味着您可以在需要时恢复它们，但这些文件将不再受版本控制的保护。

fossil-forget命令的语法如下：

```
fossil forget [OPTIONS] FILE1 ?FILE2 ...?
```

其中，OPTIONS是可选的附加选项，可以控制操作的行为。例如，使用"-n"选项可以列出将被忘记的文件，但不执行实际删除。

您可以将多个文件作为参数传递给fossil-forget命令，以一次性从版本控制系统中删除它们，例如：

```
fossil forget file1.txt file2.txt
```

该命令将从版本控制系统中删除"file1.txt"和"file2.txt"两个文件。

请注意，当您忘记文件时，除非您使用"-f"选项强制覆盖，否则fossil-version控制系统将自动创建一个备份文件，作为删除的文件的最后一个版本的副本。这可以避免不小心删除重要的文件而导致数据丢失。 

## tldr 
 
> 这是 `fossil rm` 命令的一个别名。
> 更多信息：<https://fossil-scm.org/home/help/forget>.

- 原命令的文档在：

`tldr fossil rm`
