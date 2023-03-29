# unar 
## chatgpt 
命令 `unar` 用于从各种不同的压缩文件中提取文件。它是与 Mac OSX 兼容的一个通用解压缩器，能够解压缩多种不同类型的压缩文件，包括 RAR、ZIP、TAR、GZIP 和多种其它压缩文件格式。其中，`unar` 命令用法如下：

```
unar [option] archive.[rar|zip|tar|gz|bz2|7z|exe|sit|sitx|lzma|ace|cab|deb|rpm|cpio|pdf|iso|cdr|dmg|bzip2|xar|arp]
```

其中，`archive.[rar|zip|tar|gz|bz2|7z|exe|sit|sitx|lzma|ace|cab|deb|rpm|cpio|pdf|iso|cdr|dmg|bzip2|xar|arp]` 表示将要被解压缩的压缩文件。`option` 为可选项，下面是常用的一些选项：

- `-d DIRECTORY, --directory DIRECTORY`：指定解压缩后的文件存储目录，默认与压缩文件在同一目录。
- `-e, --extract`：提取所有文件而不仅仅是文件夹。
- `-f, --force`：强制替换已存在的文件。
- `-p PASSWORD, --password PASSWORD`：指定密码，以解压受密码保护的文件。

示例：
```
unar file.zip                  # 解压 ZIP 文件
unar -d /home userfile.rar     # 解压 RAR 文件到 /home 目录下
unar -e file.gz                # 提取 GZIP 文件中的所有内容
unar -f myfile.tar             # 强制替换已存在的 TAR 文件
unar -p somepassword file.7z   # 解压受密码保护的 7Z 文件
```

总之，`unar` 是一个非常实用的工具，可以轻松解压多种压缩文件，为用户提供了方便快捷的文件管理体验。 

## tldr 
 
> 从归档文件中提取内容。
> 更多信息：<https://manned.org/unar>.

- 提取一个归档文件到当前目录：

`unar {{归档文件}}`

- 提取一个归档文件到指定目录：

`unar -o {{路径/到/目录}} {{归档文件}}`

- 如果要提取的文件已经存在，则总是覆盖：

`unar -f {{归档文件}}`

- 如果要提取的文件已经存在，则总是重命名：

`unar -r {{归档文件}}`

- 如果要提取的文件已经存在，则总是跳过：

`unar -s {{归档文件}}`
