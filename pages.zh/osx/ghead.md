# ghead 
## chatgpt 
`ghead`是`coreutils`软件集中的一部分，通常在Linux和Mac OS X操作系统中预装 。它是`head`命令的一个变种，可以在文件中显示头部的前几行。其中“g”代表“GNU”，意味着此命令由GNU贡献者创建和维护。

`ghead`的语法与`head`命令的语法相同，其命令格式如下：

```
ghead [OPTION]... [FILE]...
```

`ghead`命令的常用选项包括：

- `-c, --bytes=[-]NUM`：该选项显示文件的第几个字节或字节范围，NUM表示从文件前端的第几个字节开始，可以带有“-”表示从文件的末尾向前数
- `-n, --lines=[-]NUM`：该选项显示文件的前几行或行的范围，NUM表示要显示的行数，可以带有“-”表示从文件尾向前数
- `-q, --quiet, --silent`：该选项抑制警告信息。
- `-v, --verbose`：该选项详细输出提示信息。

`ghead`命令的使用示例：

1. 显示文件头2行

```
ghead -n 2 file.txt
```

2. 显示文件头500字节

```
ghead -c 500 file.txt
```

3. 显示文件头10行到20行

```
ghead -n 20 file.txt | tail -n +11
```

说明：首先使用`ghead`将文件前20行全部显示出来，然后再用`tail`命令从第11行开始显示，这样就相当于显示文件的第10到20行了。 

## tldr 
 
> 这是 `-p linux head` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux head`
