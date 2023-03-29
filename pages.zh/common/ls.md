# ls 
## chatgpt 
命令 "ls" 用于列出当前工作目录中的文件和子目录。

它的语法为：

```
ls [选项] [文件/目录]
```

其中，“选项”可以用来修改输出的格式或行为，而“文件/目录”可以是单个文件或目录的名称，也可以是用空格分隔的多个名称。

一些常用的选项和参数：

- `-l`：以长格式（详细信息）显示文件或目录。
- `-a`：显示隐藏文件或目录。
- `-h`：人类可读格式显示文件或目录大小。
- `-d`：仅显示目录本身，而不是其中的文件。
- `-R`：递归显示子目录中的文件和目录。

例如，以下命令将显示当前工作目录中的所有文件和子目录：

```
ls
```

而以下命令将显示当前工作目录中的所有文件和子目录，并以长格式显示：

```
ls -l
```

最后，附加一个名称参数将仅显示该文件或目录的信息，例如：

```
ls /etc
``` 

## tldr 
 
> 列出目录中的内容。
> 更多信息：<https://www.gnu.org/software/coreutils/ls>.

- 列出目录中的文件，每个文件占一行：

`ls -1`

- 列出包含隐藏文件的所有文件：

`ls -a`

- 列出所有文件，如果是目录，则在目录名后面加上「/」：

`ls -F`

- 列出包含隐藏文件的所有文件信息，包括权限，所有者，大小和修改日期：

`ls -la`

- 列出所有文件信息，大小用人类可读的单位表示（KiB, MiB, GiB）：

`ls -lh`

- 列出所有文件信息，按大小降序排序：

`ls -lS`

- 列出所有文件信息，按修改日期从旧到新排序：

`ls -ltr`

- 只列出目录：

`ls -d */`