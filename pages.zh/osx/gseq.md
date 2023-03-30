# gseq 
## chatgpt 
gseq是一个用于生成序列的命令。其具体用法如下：

```
gseq [OPTION]... LAST
```

其中LAST表示序列的最后一个数，而OPTION表示gseq命令的选项。

常用的选项包括：

- -f, --format=FORMAT：指定输出格式，其中FORMAT可以是C语言的格式化字符串。
- -w, --equal-width=WIDTH：指定输出的数字宽度，多余的数字会用0填充。
- -s, --separator=STRING：指定数字之间的分隔符。
- -r, --reverse：反向输出序列。

例如，执行命令`gseq -s , -f %03d -w 2 10`可以得到如下输出：

```
01,02,03,04,05,06,07,08,09,10
```

其中-s ,指定数字之间用逗号隔开，-f %03d指定输出的数字格式为3位数并用0填充，-w 2指定输出的数字宽度为2位数。 

## tldr 
 
> 这是 `-p linux seq` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux seq`
