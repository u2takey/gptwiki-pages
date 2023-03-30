# gbase64 
## chatgpt 
gbase64是一个Linux命令行工具，用于将二进制数据编码成Base64字符串。Base64编码是一种将二进制数据转换为可打印ASCII文本的编码方式，它使用64个字符（A-Z、a-z、0-9和“+”、“/”）来表示任意长度的文本，安全可靠，可在邮件传输和数据存储等方面广泛应用。

gbase64命令的语法如下：

```
gbase64 [选项] [文件...]
```

其中，常用的选项包括：

- -d： 解码Base64字符串到二进制数据。
- -w <列数>： 指定每行的列数。

使用gbase64命令的示例：

1. 将文本字符串编码为Base64格式：

```
$ echo "Hello World" | gbase64
SGVsbG8gV29ybGQK
```

2. 将文件内容编码为Base64格式：

```
$ gbase64 hello.txt > hello.b64
```

3. 解码Base64格式的文件或字符串：

```
$ gbase64 -d hello.b64 > hello.txt
$ echo "SGVsbG8gV29ybGQK" | gbase64 -d
Hello World
```

4. 指定每行的列数：

```
$ echo "Hello World" | gbase64 -w 10
SGVsbG8gVw
d29ybGQK
```

以上是gbase64命令的详细解释，它是一种非常实用的命令行工具。 

## tldr 
 
> 这是 `-p linux base64` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux base64`
