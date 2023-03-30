# gsha384sum 
## chatgpt 
gsha384sum是一个Linux命令，主要用于计算文件的SHA-384哈希值。

SHA-384是散列算法中的一种，它能够将任意长度的输入数据生成一个384位（48字节）的散列值。SHA-384具有高度安全性和不可逆性，用于验证文件完整性和检查数据传输。

gsha384sum命令用法如下：

```
gsha384sum [选项] [文件名]
```

常用选项：

- `-c, --check`：读取文件中的 SHA-384 校验和，验证每个文件的正确性。
- `-t, --text`：将二进制文件视为纯文本文件进行处理。

示例：

1. 计算文件的SHA-384哈希值

```
gsha384sum filename
```

2. 计算多个文件的SHA-384哈希值

```
gsha384sum file1 file2 file3
```

3. 验证文件的SHA-384哈希值

```
gsha384sum -c checksum.txt
```

其中checksum.txt是一个包含SHA-384哈希值的文件，可以通过gsha384sum命令进行验证。 

## tldr 
 
> 这是 `-p linux sha384sum` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux sha384sum`
