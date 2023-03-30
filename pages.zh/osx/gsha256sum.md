# gsha256sum 
## chatgpt 
gsha256sum是一个Linux命令，用于计算并显示一个或多个文件的SHA-256哈希值，该哈希算法可以将数据块转换为一个固定长度的唯一值，从而保证数据完整性和安全性。

gsha256sum的语法如下：

```
gsha256sum [OPTION]... [FILE]...
```

可用选项包括：

- -b或--binary：以二进制模式输出文件的哈希值。
- -c或--check：从文件中读取哈希值并检查它们是否与文件的实际哈希值匹配。
- -t或--text：以文本模式输出文件的哈希值（默认模式）。

使用gsha256sum命令的基本步骤如下：

1. 打开终端/命令行窗口。
2. 确定要计算哈希值的文件路径。
3. 输入gsha256sum命令的语法，包括选项和文件路径。
4. 按Enter键执行命令。
5. 等待程序计算和显示哈希值。

例如，以下命令将计算文件"testfile.txt"的SHA-256哈希值并以文本模式输出：

```
gsha256sum testfile.txt
```

输出结果将类似于：

```
1a79a4d60de6718e8e5b326e338ae533
```

其中，"1a79a4d60de6718e8e5b326e338ae533"是testfile.txt文件的SHA-256哈希值。 

## tldr 
 
> 这是 `-p linux sha256sum` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux sha256sum`
