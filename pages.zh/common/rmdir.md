# rmdir 
## chatgpt 
rmdir是一个Unix/Linux命令，用于删除一个空目录。

其基本语法如下：

```
rmdir [OPTIONS] DIRECTORY
```

其中：

- OPTIONS：可选项，可以指定一些选项，如-r等。
- DIRECTORY：必选参数，指定要删除的目录。

该命令需要特别注意的是：

- 不能删除非空目录。如果要删除非空目录，需要使用rm命令。
- 删除目录前应该先备份数据，以免误删除。
- 删除操作无法恢复，一旦删除就无法恢复，因此请谨慎操作。

常用选项：

- -p 或 --parents：递归删除空目录，如果指定的目录结构不存在，则会递归删除路径中的父目录，直到找到存在的目录位置。
- -v 或 --verbose：显示目录删除过程。 

## tldr 
 
> 删除一个目录。
> 更多信息：<https://www.gnu.org/software/coreutils/rmdir>.

- 删除空目录，使用 `rm -r` 删除非空目录：

`rmdir {{路径/到/目录}}`

- 删除目标及其父目录（对嵌套的目录有用）：

`rmdir -p {{路径/到/目录}}`