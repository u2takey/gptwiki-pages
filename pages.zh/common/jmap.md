# jmap 
## chatgpt 
jmap是Java Memory Map工具的一个命令行工具，用于生成Java虚拟机(Java Virtual Machine, JVM)中的内存快照并分析这些内存快照。jmap可以在运行时打印出Java堆的内存情况，包括Java堆中对象的总数、数量、占用的空间大小等信息，还可以分析哪些对象占用了大量的空间，从而帮助开发人员识别具体的Java内存泄漏问题。

jmap的常用选项包括：

1. -dump：生成Java堆转储文件

2. -F：当jmap进程无响应时，强制生成内存转储文件

3. -heap：打印出Java堆内存使用情况

4. -histo：打印出Java堆中各个对象类型的数量、内存占用大小等信息

5. -J：将选项传递给底层的JVM

jmap工具的输出结果可以作为其他调试和分析工具的输入，例如jvisualvm和Eclipse Memory Analyzer等，可帮助开发人员更好地理解与优化Java程序的内存使用情况。 

## tldr 
 
> Java 内存映射工具。
> 更多信息：<https://docs.oracle.com/javase/7/docs/technotes/tools/share/jmap.html>.

- 打印 Java 进程的共享对象映射（类似 pmap 的输出）：

`jmap {{Java 进程号}}`

- 打印堆摘要信息：

`jmap -heap {{Java 进程号}}`

- 按类型打印堆使用的直方图：

`jmap -histo {{Java 进程号}}`

- 将堆的内容转储到二进制文件中以使用 jhat 进行分析：

`jmap -dump:format=b,file={{导出文件名}} {{Java 进程号}}`
