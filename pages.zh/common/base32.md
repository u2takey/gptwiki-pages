# base32 
## chatgpt 
base32命令是一个Linux命令行工具，用于将二进制数据编码为基于32个字符的文本格式，以便于在邮件传输、数据备份、密钥管理等方面的广泛应用。

base32命令的语法格式为：

```shell
base32 [选项]... [文件名]...
```

命令选项：

- -d：解码选项，用于将文本数据解码为二进制格式。
- -i：输入文件选项，指定要编码或解码的文件名，如果省略则表示从标准输入读取数据。
- -o：输出文件选项，指定编码或解码结果输出到的文件名，如果省略则输出到标准输出。
- -w：行宽选项，指定每行输出多少个字符，默认为76个。

使用示例：

1. 将一个二进制文件编码为base32文本格式：

```shell
base32 binaryfile > base32file.txt
```

2. 将一个base32文本文件解码为二进制格式：

```shell
base32 -d base32file.txt > binaryfile
```

3. 将标准输入数据编码为base32文本格式：

```shell
echo "hello world" | base32
```

4. 将一个长度为100的随机数编码为base32格式输出：

```shell
dd if=/dev/urandom bs=100 count=1 | base32
``` 

## tldr 
 
> 将文件或标准输入编码到 Base32 或从 Base32 解码为标准输出。
> 更多信息：<https://www.gnu.org/software/coreutils/base32>.

- 编码一个文件：

`base32 {{文件名}}`

- 解码一个文件：

`base32 --decode {{文件名}}`

- 从标准输入编码：

`{{某指令}} | base32`

- 将标准输入解码：

`{{某指令}} | base32 --decode`
