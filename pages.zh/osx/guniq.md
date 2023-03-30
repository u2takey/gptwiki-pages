# guniq 
## chatgpt 
guniq是Linux/Unix操作系统中的一个命令，用于在文本文件中查找并删除重复的行。它的语法格式如下：

```
guniq [选项] [输入文件]
```

常用选项包括：

- -c，--count：在输出中列出每行重复的次数。
- -d，--repeated：仅显示重复的行。
- -u，--unique：仅显示不重复的行。
- -i，--ignore-case：忽略大小写进行比较。
- -s num，--skip-chars=num：从行开头的第num个字符开始比较。

例如，假设我们有一个文本文件test.txt，内容如下：

```
hello
world
world
foo
bar
foo
```

如果我们想要只显示不重复的行，可以运行以下命令：

```
guniq -u test.txt
```

它将只显示如下内容：

```
hello
world
foo
bar
```

如果我们想要显示重复的行及其出现次数，可以运行以下命令：

```
guniq -c test.txt
```

它将输出如下内容：

```
      1 hello
      2 world
      2 foo
      1 bar
``` 

## tldr 
 
> 这是 `-p linux uniq` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux uniq`
