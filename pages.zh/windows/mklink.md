# mklink 
## chatgpt 
mklink（make link） 是Windows 命令行中的一个工具，用于创建或修改指向文件或文件夹的符号链接（也称为软链接或符号连接）。

符号链接是一种特殊的文件或文件夹，它包含一个指向另一个文件或文件夹的路径。这种链接不是实际文件或文件夹的副本，而是指向原始文件或文件夹的快捷方式。这对于保存空间和在系统内维护多个版本的相同文件很有用。

使用 mklink 命令创建符号链接的基本语法是：

```
mklink [options] <link> <target>
```

其中，`<link>` 是要创建的符号链接的名称，`<target>` 是符号链接指向的目标（可以是文件或文件夹）的路径。

一些常见的选项包括：

- `/D` - 创建目录符号链接而不是文件符号链接。
- `/J` - 创建目录的联接点（junction point）而不是符号链接。联接点类似于符号链接，但是只能指向目录。
- `/H` - 创建硬链接而不是符号链接。硬链接不同于符号链接，它们是实际文件系统中的物理副本，不支持跨分区链接。

以下是几个示例：

1. 创建文件符号链接

```
mklink filename.txt C:\path\to\file
```

这将创建一个名为 `filename.txt` 的符号链接，指向 `C:\path\to\file`。

2. 创建目录符号链接

```
mklink /D directory C:\path\to\dir
```

这将创建一个名为 `directory` 的目录符号链接，指向 `C:\path\to\dir`。

3. 创建目录联接点

```
mklink /J directory C:\path\to\dir
```

这将创建一个名为 `directory` 的目录联接点，指向 `C:\path\to\dir`。

需要注意的是，创建符号链接需要管理员权限。在非管理员权限下执行该命令会导致“访问被拒绝”的错误。 

## tldr 
 
> 创建符号链接。
> 更多信息：<https://learn.microsoft.com/windows-server/administration/windows-commands/mklink>.

- 创建指向文件的符号链接：

`mklink {{链接文件的路径}} {{源文件路径}}`

- 创建指向目录的符号链接：

`mklink /d {{链接文件的路径}} {{源目录路径}}`

- 创建指向文件的硬链接：

`mklink /h {{链接文件的路径}} {{源目录路径}}`

- 创建目录链接：

`mklink /j {{链接文件的路径}} {{源目录路径}}`
