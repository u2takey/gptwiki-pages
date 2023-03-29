# base64 
## chatgpt 
base64命令是一种用于将二进制数据编码为ASCII字符的工具。具体来说，它将3个字节的数据组合为4个6位字节（也就是24位），然后将每个6位字节映射到ASCII字符集中的相应字符，以生成一个由ASCII字符组成的编码字符串。Base64编码不是对数据进行加密，而只是一种编码方法。

base64命令可以用于以下情况：

1. 将二进制数据编码为文本格式，以便在文本协议中进行传输

2. 对二进制数据进行编码，以便在文本编辑器中进行查看和编辑

3. 对二进制数据进行编码，以便在电子邮件和Web表单等场景中进行传输

一般而言，base64命令有两种基本用法：

1. 编码：将二进制数据转换为ASCII字符
``` 
  base64 < filename #将文件内容 base64 编码并输出到终端
  base64 -w 0 filename #将文件内容 base64 编码, 不使用折行 & 输出到终端
```
2. 解码：将ASCII字符转换为二进制数据 
```
 base64 -d < filename #将文件内容进行 base64 解码并输出到终端
 base64 -D < filename #将文件内容进行 base64 等价性解码并输出到终端
``` 
选项-w表示输出的行宽，-d用于解码，-D可用于等价性解码。

例如，以下是将一个名为input.bin的二进制文件编码为base64字符串的命令：
```
base64 input.bin > output.txt
```
这将把编码后的字符串输出到output.txt文件中。反过来，以下是从base64字符串解码为二进制文件的命令：
```
base64 -d input.txt > output.bin
```
这将从input.txt中读取编码字符串，并将解码后的二进制数据写入output.bin文件中。 

## tldr 
 
> 将文件或标准输入编码到 Base64 或从 Base64 解码为标准输出。
> 更多信息：<https://www.gnu.org/software/coreutils/base64>.

- 编码一个文件：

`base64 {{文件名}}`

- 解码一个文件：

`base64 --decode {{文件名}}`

- 从标准输入编码：

`{{某指令}} | base64`

- 将标准输入解码：

`{{某指令}} | base64 --decode`
