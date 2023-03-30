# gstdbuf 
## chatgpt 
命令`gstdbuf`是Glibc库中的命令，用于执行其他命令时控制标准输入、标准输出和标准错误流的缓冲区大小。

它的一般语法如下：

```
gstdbuf OPTION... COMMAND
```

其中，`OPTION`表示选项，`COMMAND`表示要执行的命令。

`gstdbuf`的选项如下：

- `--help`：显示帮助。
- `--output-open-mode MODE`：设置标准输出流的打开模式，可选的值有`r`（只读），`w`（只写）、`a`（追加）和`x`（排他）。
- `--input MODE`：设置标准输入流的类型，可选的值有`fully-buffered`（默认，完全缓冲）、`line-buffered`（行缓冲）和`unbuffered`（无缓冲）。
- `--output MODE`：设置标准输出流的类型，可选的值同上。
- `--error MODE`：设置标准错误流的类型，可选的值同上。

`gstdbuf`命令的作用类似于`stdbuf`命令，在执行其他命令时可以控制缓冲区，但是它能够同时控制标准输入、输出和错误流的缓冲区大小。此外，`gstdbuf`命令默认按照完全缓冲的方式执行命令，而`stdbuf`命令默认行缓冲方式执行命令。 

## tldr 
 
> 这是 `-p linux stdbuf` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux stdbuf`
