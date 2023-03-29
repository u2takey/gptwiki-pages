# mac2unix 
## chatgpt 
mac2unix命令用于将Mac OS X和早期Mac OS系统生成的文本文件格式转换为Unix或Linux系统可读的格式。它通常用于在不同操作系统之间共享文本文件时使用。

使用mac2unix命令需要在终端中输入以下命令：

```
mac2unix [选项] 文件
```

其中选项可以是以下之一：

- -v：启用详细模式，显示每个转换的文件名。
- -h：显示命令帮助信息。

文件参数指定要转换的文件的路径。可以指定单个文件或使用通配符指定多个文件。

例如，以下命令将名为file.txt的Mac格式文本文件转换为Unix格式：

```
mac2unix file.txt
```

转换后，文件的行末将以Unix格式的换行符（LF）表示，而不是Mac格式的换行符（CR）。

注意：mac2unix命令只是一个简单的脚本，它基本上是一个在命令行下执行sed命令的简化方式。在某些Linux发行版中可能没有自带mac2unix工具，但是可以使用sed命令实现相同的效果。 

## tldr 
 
> 将 macOS 样式的行尾更改为 Unix 样式。
> 用 LF 替换 CR.
> 更多信息：<https://waterlan.home.xs4all.nl/dos2unix.html>.

- 更改文件的行尾：

`mac2unix {{文件名}}`

- 使用 Unix 样式的行尾创建副本：

`mac2unix -n {{文件名}} {{新文件名}}`
