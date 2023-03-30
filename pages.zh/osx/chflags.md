# chflags 
## chatgpt 
chflags是一个命令行工具，用于更改文件或目录的访问权限标志。

标志是文件系统中用于控制文件和目录访问的一种机制。它们是在文件系统中的每个目录项上设置的，以决定用户是否可以读取、写入、执行或删除文件。标志还可以控制文件或目录是否可以被其他用户或进程修改或删除。

chflags命令可用于更改常见的访问权限标志：

- -R：递归地更改目录及其子目录下的标志
- -v：显示执行结果
- -f：忽略错误信息

以下是chflags可用的标志（或者叫参数）：

- uchg：防止其他用户或进程修改或删除文件
- uunlnk：防止其他用户或进程删除文件
- hidden：将文件或目录隐藏
- schg：防止文件或目录被修改或删除
- sappnd：确保只有创建者可以添加内容到文件或目录
- sunlnk：防止文件或目录被删除

例如，要将文件“example.txt”的标志设置为“uchg”，可以使用以下命令：

```
chflags uchg example.txt
```

要将目录“myFolder”的标志设置为“hidden”，可以使用以下命令：

```
chflags hidden myFolder
```

需要注意的是，更改标志可能会影响文件或目录的正常运行，因此应该谨慎使用。建议在更改前备份相关文件或目录。 

## tldr 
 
> 更改文件或文件夹的标志。
> 更多信息：<https://ss64.com/osx/chflags.html>.

- 给文件设置 hidden（隐藏）标签：

`chflags {{hidden}} {{文件路径}}`

- 取消文件的 hidden 标签：

`chflags {{hidden}} {{文件路径}}`

- 递归地给文件夹中每个文件设置 uchg 标志：

`chflags -R {{uchg}} {{文件夹路径}}`

- 递归地撤销文件夹中每个文件设置的 uchg 标志：

`chflags -R {{nouchg}} {{文件夹路径}}`
