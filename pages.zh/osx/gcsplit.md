# gcsplit 
## chatgpt 
gcsplit命令是在Unix或Linux系统中用来分割文件的。它将一个输入文件分割成多个较小的文件，每个文件包含从输入文件中选择的特定数据段。

gcsplit命令的语法如下：

```
gcsplit [OPTION] INPUT PREFIX [SUFFIX]
```

其中，[OPTION]是可选的命令行选项，[INPUT]是输入文件的名称，[PREFIX]是输出文件的前缀，[SUFFIX]是输出文件名的后缀。

以下是gcsplit命令的一些常见选项：

- -f：指定输出文件名前缀。
- -b：指定输出文件名后缀的格式。
- -n：指定输出文件名后缀的数字位数。
- -k：保留分割文件时匹配项的行数在输出文件中。
- -s：不打印未匹配的数据行。

示例：

假设有一个名为example.txt的文件，其内容如下：

```
line1
line2
line3
line4
line5
```

现在，我们将使用gcsplit命令将其分割为两个文件，每个文件包含两行。命令如下：

```
gcsplit -l 2 example.txt example_
```

这将生成两个文件：example_aa和example_ab，其内容如下：

example_aa：

```
line1
line2
```

example_ab：

```
line3
line4
```

注意，在命令中使用了“-l”选项来指定每个输出文件的行数。另外，我们没有指定输出文件名后缀的格式和数字位数，因为这些选项使用默认设置即可。 

## tldr 
 
> 这是 `-p linux csplit` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux csplit`
