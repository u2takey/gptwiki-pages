# gsha1sum 
## chatgpt 
gsha1sum 是一个 Unix 和 Linux 操作系统上的命令行工具，用于计算文件的 SHA1 校验和。

SHA1 是一种常用的哈希算法，用于计算文件的数字指纹，也称为校验和。通过计算文件的 SHA1 校验和，可以验证文件的完整性和一致性，以及检测文件是否被篡改或损坏。

gsha1sum 命令的语法格式如下：

```
gsha1sum [OPTION]... [FILE]...
```

其中，`OPTION` 是可选参数，用于控制 gsha1sum 的行为，`FILE` 是待计算校验和的文件名列表。

常用的选项包括：

- `-b` 或 `--binary`：以二进制模式计算校验和（默认以文本模式计算）。
- `-c` 或 `--check`：校验给定的校验和文件。
- `-t` 或 `--text`：以文本模式计算校验和（默认以二进制模式计算）。

使用示例：

计算单个文件的 SHA1 校验和：

```
gsha1sum file.txt
```

计算多个文件的 SHA1 校验和：

```
gsha1sum file1.txt file2.txt
```

计算二进制文件的 SHA1 校验和：

```
gsha1sum -b binaryfile.dat
```

校验给定的校验和文件：

```
gsha1sum -c sha1sum.txt
```

计算文件列表中所有文件的 SHA1 校验和，并将结果保存到文件中：

```
gsha1sum * > sha1sum.txt
``` 

## tldr 
 
> 这是 `-p linux sha1sum` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux sha1sum`
