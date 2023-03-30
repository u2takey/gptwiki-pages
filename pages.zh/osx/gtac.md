# gtac 
## chatgpt 
gtac是Linux/Unix操作系统下的一个命令行工具，用于反向显示文件内容。它的作用是将文件中的每一行反向输出，也就是以最后一行开始，逐行向上输出，即逆序输出文件内容。

使用语法：

```
gtac [OPTION]… [FILE]…
```

参数说明：

- OPTION：选项参数
- FILE：待处理文件名

常用选项：

- -b, --before：在每行前添加分隔符
- -s, --separator=STRING：使用指定的分隔符代替默认的换行符
- -T, --no-trailing：忽略文件末尾的空行
- --help：显示帮助信息
- --version：显示版本信息

示例：

1. 将文件file.txt中的每一行反向输出

```
gtac file.txt
```

2. 在每一行前添加分隔符'+'并反向输出文件file.txt

```
gtac -b "+" file.txt
```

3. 使用分隔符'-'代替默认的换行符并反向输出文件file.txt

```
gtac -s "-" file.txt
```

4. 忽略文件末尾的空行并反向输出文件file.txt

```
gtac -T file.txt
``` 

## tldr 
 
> 这是 `-p linux tac` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux tac`
