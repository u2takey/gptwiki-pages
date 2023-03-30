# gmkdir 
## chatgpt 
很抱歉，这个命令“gmkdir”在常见的 Linux 和 Unix 操作系统中不存在。可能您想要了解的命令是 mkdir，这是一个基本的 Linux 和 Unix 命令，用于创建一个新目录或文件夹。

使用 mkdir 命令时，您需要输入要创建的新目录的名称，例如：

```
mkdir new_folder
```

如果您需要在当前目录下创建一个新目录，可以省略目录的完整路径：

```
mkdir folder_name
```

如果您需要同时创建一个或多个子目录，可以使用 -p 选项：

```
mkdir -p parent/child/grandchild
```

这将在当前目录下创建一个名为 parent 的目录，其中包含子目录 child 和 grandchild。

为了防止其他用户或程序意外地更改创建的目录，请使用 chmod 命令来更改新目录的权限：

```
chmod 755 new_folder
```

这将使当前用户能够读取、写入和访问该目录，而其他用户只能读取和访问该目录。 

## tldr 
 
> 这是 `-p linux mkdir` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux mkdir`
