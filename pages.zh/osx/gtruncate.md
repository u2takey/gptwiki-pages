# gtruncate 
## chatgpt 
`gtruncate`是一个GNU Coreutils工具，用于截断文件中的内容。它可以通过指定文件的大小或以指定单位的字节数来进行截断。

命令语法：

```
gtruncate [OPTION]... SIZE FILE...
```

其中，`SIZE`参数指定截断后的大小，可以使用诸如“1M”、“500K”、“10G”等格式来指定文件大小。`FILE`参数则指定要截断的文件名。

常用选项包括：

- `-s, --size=SIZE`：指定截断后的文件大小；
- `-c, --no-create`：指定如果文件不存在则不进行创建；
- `-o, --io-blocks`：使用I/O块大小而不是字节数来指定截断大小；
- `-r, --reference=REF_FILE`：将截断大小设置为参考文件的大小；
- `-v, --verbose`：显示每个截断文件的名称。

例如，要将文件`example.txt`截断到1 MB的大小，可以使用以下命令：

```
gtruncate -s 1M example.txt
```

当文件`example.txt`的大小大于1 MB时，`gtruncate`会删除文件的末尾字节，从而将其大小截断到1 MB。如果文件大小小于1 MB，则不执行任何操作。

该命令也可以通过使用负数值而不是大小来截断文件。例如，要删除文件`example.txt`的末尾10 MB，可以使用以下命令：

```
gtruncate -s -10M example.txt
```

当文件`example.txt`的大小小于10 MB时，`gtruncate`会删除整个文件。否则，它会删除文件的末尾10 MB。 

## tldr 
 
> 这是 `-p linux truncate` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux truncate`
