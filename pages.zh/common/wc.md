# wc 
## chatgpt 
wc 是一个 Linux/Unix 系统命令，用于计算文件中的字节数、字数、行数等信息。它的使用方法为：

`wc [选项] [文件名]`

其中，选项包括：

- `-c`：统计字节数；
- `-w`：统计单词数；
- `-l`：统计行数；

默认情况下，使用 wc 命令不带选项时，会同时显示文件的行数、单词数和字节数，格式如下：

```
行数    单词数    字节数    文件名
```

用法示例：

统计一个文件的行数、单词数和字节数：

```
wc filename.txt
```

只统计行数：

```
wc -l filename.txt
```

只统计单词数：

```
wc -w filename.txt
```

只统计字节数：

```
wc -c filename.txt
``` 

## tldr 
 
> 计数行、单词或字节。
> 更多信息：<https://www.gnu.org/software/coreutils/wc>.

- 计数文件中的行数：

`wc -l {{文件}}`

- 计数文件中的单词数：

`wc -w {{文件}}`

- 计数文件中的字符（字节）：

`wc -c {{文件}}`

- 计数文件中的字符数（考虑所有多字节的字符）：

`wc -m {{文件}}`

- 使用标准输入，按顺序计数行、单词和字符（字节）：

`{{find .}} | wc`
