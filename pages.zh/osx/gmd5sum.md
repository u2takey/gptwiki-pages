# gmd5sum 
## chatgpt 
gmd5sum是一个Linux命令，用于计算文件的MD5哈希值。MD5哈希值是一个固定长度的唯一字符串，可以用于验证文件的完整性和安全性。

gmd5sum命令的语法如下：

```
gmd5sum [options] [file(s)]
```

参数说明：

- options：可选参数，用于控制gmd5sum命令的行为。具体选项请使用man gmd5sum命令查看。
- file(s)：要计算哈希值的文件。可以指定一个或多个文件名称或通配符。

对指定的文件执行gmd5sum命令后，将会输出每个文件的MD5哈希值，并在每行开头添加SHA256哈希算法所得的哈希值作为前缀。例如：

```
$ gmd5sum file.txt
d690b691fc63e7fc832b06634febba59 d2ffcd2706fabe19f5cb3e9ba2c0505014f12d4df93c142626f414182adcb24a  file.txt
```

其中，第一个哈希值是文件的MD5值，第二个哈希值是SHA256哈希值的前缀。如果需要单独输出MD5值，可以使用如下命令：

```
$ gmd5sum file.txt | cut -d ' ' -f 1
d690b691fc63e7fc832b06634febba59
``` 

## tldr 
 
> 这是 `-p linux md5sum` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux md5sum`
