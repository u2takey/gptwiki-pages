# gsha224sum 
## chatgpt 
gsha224sum命令是一个Linux命令，用于计算和检查SHA-224哈希值。它可用于验证文件或文本的完整性，以确保它们在传输过程中没有被篡改或损坏。

该命令的一般语法为：

gsha224sum [选项] [文件名]

选项包括：

- --check：用于从文件中读取SHA-224值并检查文件的哈希值是否匹配。
- --status：用于从文件中读取SHA-224值并显示检查成功或失败的信息。
- --quiet：用于禁用命令的所有输出，仅返回退出码来表示哈希值的匹配情况。

例如，如果要计算文件example.txt的SHA-224哈希值，可以使用以下命令：

gsha224sum example.txt

如果要从文件checksum.txt中读取SHA-224哈希值，并检查example.txt文件的哈希值是否匹配，则可以使用以下命令：

gsha224sum --check --status checksum.txt

这将从checksum.txt文件中读取哈希值，并在example.txt文件的哈希值与读取的哈希值匹配时显示“OK”。如果哈希值不匹配，则显示“FAILED”。 

## tldr 
 
> 这是 `-p linux sha224sum` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux sha224sum`
