# gbase32 
## chatgpt 
gbase32是一个基于Base32编码算法的命令行工具，用于将文本或二进制数据编码为Base32格式的字符串。

Base32是一种将8位数据字节转换为5位数据字节的编码方式，使用字母A-Z和数字2-7的组合表示数据。这种编码方式通常用于电子邮件、网络传输和存储数据，因为它可以有效地压缩数据并减少传输时的错误率。

使用gbase32命令可以将输入的文本或二进制数据转换为Base32格式的字符串。例如，要将一个文本文件编码为Base32格式，可以使用以下命令：

```
gbase32 file.txt > file.txt.b32
```

这会将file.txt文件编码为Base32格式，并将结果输出到file.txt.b32文件中。

另外，gbase32还可以从Base32格式解码数据。例如，要将一个Base32编码的文件解码为原始文件，可以使用以下命令：

```
gbase32 -d file.txt.b32 > file.txt
```

这会将file.txt.b32文件解码为原始文件，并将结果输出到file.txt文件中。 

## tldr 
 
> 这是 `-p linux base32` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux base32`
