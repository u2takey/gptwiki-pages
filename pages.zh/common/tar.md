# tar 
## chatgpt 
tar 命令是一个非常常用的 Linux 命令，用于打包和压缩文件和目录。具体解释如下：

命令格式：

```
tar [参数选项] [打包后文件名] [需要打包的文件列表/目录列表]
```

常用的参数选项：

- `-c`：创建一份新的 tar 归档文件。
- `-x`：从 tar 归档文件中解压出文件。
- `-t`：列出 tar 归档文件中的内容。
- `-v`：输出详细信息。
- `-f`：指定归档文件的名称。

常用的实例：

1. 打包文件

将目录下所有文件打包为 tar 包：

```
tar -cvf files.tar *
```

2. 压缩文件

将一个文件打 tar 包并压缩为 gzip 格式：

```
tar -czvf file.tar.gz file.txt
```

3. 解压文件

解压 tar 包：

```
tar -xvf file.tar
```

4. 列出压缩包的内容

列出 tar 包中包含的文件：

```
tar -tvf file.tar.gz
```

5. 追加文件到 tar 包中

将新文件追加到 tar 包中：

```
tar -rvf file.tar newfile.txt
```

6. 只解压部分文件

只解压 tar 包中的指定文件：

```
tar -xvf file.tar file1.txt file2.txt
```

总的来说，tar 命令是一个非常强大的命令，可以实现各种压缩和打包操作。有了 tar 命令，文件的备份和传输就变得非常方便了。 

## tldr 
 
> 归档实用程序。
> 通常与压缩方法结合使用，例如 gzip 或 bzip2.
> 更多信息：<https://www.gnu.org/software/tar>.

- 创建存档并将其写入文件：

`tar cf {{target.tar}} {{file1}} {{file2}} {{file3}}`

- 创建一个 gzip 压缩文件并将其写入文件：

`tar czf {{target.tar.gz}} {{file1}} {{file2}} {{file3}}`

- 使用相对路径从目录创建一个 gzip 压缩文件：

`tar czf {{target.tar.gz}} --directory={{path/to/directory}} .`

- 详细地将（压缩的）存档文件提取到当前目录中：

`tar xvf {{source.tar[.gz|.bz2|.xz]}}`

- 将（压缩的）存档文件解压缩到目标目录中：

`tar xf {{source.tar[.gz|.bz2|.xz]}} --directory={{directory}}`

- 创建压缩存档并将其写入文件，使用存档后缀确定压缩程序：

`tar caf {{target.tar.xz}} {{file1}} {{file2}} {{file3}}`

- 详细列出 tar 文件的内容：

`tar tvf {{source.tar}}`

- 从存档文件中提取与模式匹配的文件：

`tar xf {{source.tar}} --wildcards "{{*.html}}"`
