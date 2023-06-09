# base64 
## chatgpt 
base64是一种将任意二进制数据表示成可打印字符的编码方式。它通常用于在网络上传输二进制数据，如图片，音频和视频等。

使用base64编码将字节序列转换成文本数据，可用于在文本邮件中传输二进制数据、在 URL 中传递数据参数等。同时，base64编码是不加密的，只是一种编码方式，安全性较差，不宜用于敏感信息的传输。

在命令行中，base64命令可以对文件或字符流进行编码或解码操作。使用base64编码可以通过以下命令：

```
base64 <输入文件>
```

可以将输入文件进行base64编码，并将编码结果输出到标准输出。

如果需要解码，可以使用以下命令：

```
base64 -d <输入文件>
```

将输入文件进行base64解码，并将解码结果输出到标准输出。

base64命令还提供了一些可选参数，如-l参数可指定编码结果每行输出的字符数，-i参数可在编码输出时插入新行。可以使用man base64命令查看完整的命令行帮助文档。 

## tldr 
 
> 使用 Base64 来进行编码和解码。
> 更多信息：<https://www.unix.com/man-page/osx/1/base64/>.

- 编码目标文件：

`base64 --input={{目标文件}}`

- 解码目标文件：

`base64 --decode --input={{base64 编码文件}}`

- 通过标准输入管道进行解码：

`echo -n {{目标字符串}} | base64`

- 解码标准输入管道内容：

`echo -n {{base64 字符串}} | base64 --decode`
