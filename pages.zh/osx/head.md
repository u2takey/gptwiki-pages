# head 
## chatgpt 
head命令是一个常用的Linux命令，它用来显示文本文件的开头若干行。

常用的语法格式为：

```
head [参数] [文件名]
```

主要参数：

- -n<number>：指定要显示的行数。
- -v：显示文件名。
- -q：不显示文件名。

例子：

```
head file.txt      #显示文件的头10行
head -n 5 file.txt #仅显示文件的头5行
head -v file.txt   #显示文件名，并显示文件的头10行
head -q file.txt   #不显示文件名，并显示文件的头10行
```

值得注意的是，可以使用head命令与其他命令或管道结合使用，以便更好地处理文本数据。一些常见用法包括：

```
命令|head     #显示命令的前10行输出
head file.txt|命令  #显示文件的前10行输出，并通过管道传递给另一个命令处理
```

总之，head命令是一个非常实用的命令，常用于查看文件的头部信息，快速浏览文件内容，以及配合管道使用获得一些信息。 

## tldr 
 
> 输出文件的开头部分。
> 更多信息：<https://ss64.com/osx/head.html>.

- 输出文件的前几行：

`head -n {{行数}} {{文件名}}`

- 输出文件的前几个字节：

`head -c {{字节数}} {{文件名}}`