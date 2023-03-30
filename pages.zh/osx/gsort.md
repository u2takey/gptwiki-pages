# gsort 
## chatgpt 
gsort是一个命令行工具，用于对文本文件进行排序。它在Linux和其他类Unix操作系统中可用。

使用gsort命令时，可以指定排序的行、字段和排序的方式。它可以按字母顺序、数字顺序、日期等进行排序。

gsort命令的语法如下：

```
gsort [OPTION]... [FILE]...
```

可用的选项包括：

- `-b`或`--ignore-leading-blanks`：忽略每行开头空格
- `-c`或`--check`：检查文件是否已按照要求排序，不排序
- `-d`或`--dictionary-order`：按字典顺序比较，忽略标点符号和空格字符
- `-f`或`--ignore-case`：忽略字符大小写
- `-h`或`--human-numeric-sort`：按照可读的数字顺序排序（例如1K、2G、3M等）
- `-i`或`--ignore-nonprinting`：忽略非打印字符
- `-n`或`--numeric-sort`：按照数值大小排序
- `-r`或`--reverse`：以逆序排序（从大到小）
- `-t`或`--field-separator`：指定字段分隔符
- `-u`或`--unique`：仅输出不重复的行

例如，要按整数大小逆序（从大到小）排序文件input.txt，可以使用以下命令：

```
gsort -rn input.txt
```

它会输出排序后的结果。 

## tldr 
 
> 这是 `-p linux sort` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux sort`
