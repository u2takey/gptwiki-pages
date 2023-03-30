# gtime 
## chatgpt 
gtime是GNU Time的缩写，它是一个UNIX/Linux命令，用于测量指定命令的执行时间。gtime命令在执行时，可以提供命令执行的实际时间，用户CPU使用时间，系统CPU使用时间，最大占用内存，缺页次数等信息。

gtime命令的语法如下：

```
gtime [OPTION]... COMMAND [ARG]...
```

其中，OPTION是可选参数，用于指定测量命令的方式和输出格式；COMMAND是要测量的命令或程序，ARG是命令的参数。

gtime命令的选项包括：

- -a 或 --append：将测量结果追加到文件中。
- -f FORMAT 或 --format=FORMAT：指定输出格式。
- -o FILE 或 --output=FILE：将测量结果输出到指定的文件中。
- -p 或 --portability：使用POSIX兼容格式输出结果。
- -v 或 --verbose：输出详细信息。

gtime命令的输出包括：

- 实际时间（real）：从命令开始到命令结束所花费的实际时间。
- 用户CPU时间（user）：命令运行时CPU所花费的时间。
- 系统CPU时间（sys）：命令在内核中运行时CPU所花费的时间。
- 最大常驻内存（max resident）：命令运行期间使用的最大常驻内存。
- 缺页总数（page faults）：命令在执行过程中发生缺页的次数。
- 总共使用的CPU时间（elapsed）：执行命令所花费的总CPU时间。

综上所述，gtime命令可以帮助用户从不同角度了解命令的执行情况，可以用来测试和比较不同命令的执行效率，找出程序瓶颈等。 

## tldr 
 
> 这是 `-p linux time` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux time`
