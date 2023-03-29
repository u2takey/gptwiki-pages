# llvm-strings 
## chatgpt 
llvm-strings是一个用于提取目标文件中ASCII和Unicode字符串的命令行工具。它是LLVM工具中的一个，它可以通过安装LLVM来获得。

使用方法：

```
llvm-strings [options] filename [...]
```

选项：

- `-a`: 提取所有字符串，包括非打印字符。
- `-n <minlen>`: 仅提取长度不小于指定值的字符串。
- `-t`: 在输出字符串前添加文件偏移量（也就是字符串在文件中的偏移量）。
- `-E <pattern>`: 使用正则表达式来过滤字符串。
- `-o <offset>`: 从指定的偏移量开始提取字符串。
- `-h`: 显示帮助文档。

示例：

```
llvm-strings -a -n 6 -t ./sample.exe
```

这个命令将会提取sample.exe中长度不小于6的所有字符串，并在每个字符串前添加偏移量。如果你的文件中有一些隐藏的ASCII或Unicode字符串，这个命令可能会将它们提取出来。 

## tldr 
 
> 这是 `strings` 命令的一个别名。

- 原命令的文档在：

`tldr strings`
