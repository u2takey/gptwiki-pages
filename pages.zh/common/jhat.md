# jhat 
## chatgpt 
jhat是Java Heap Analysis Tool的缩写，是Java Development Kit（JDK）提供的一个用于分析Java堆信息的命令行工具。

jhat的基本使用方法是：

1. 在JDK安装目录的bin目录下打开命令行窗口（Windows系统）或终端（Unix/Linux系统）。

2. 输入jhat命令，后面跟着要分析的Java堆信息文件的路径。例如：jhat /path/to/java/heap/dump/file。

3. jhat会启动一个本地HTTP服务器，并在默认端口号（7000）上监听HTTP请求。

4. 使用浏览器访问http://localhost:7000可以进入jhat的分析界面，该界面可以展示Java堆的各种信息，包括对象数量、空间使用情况、GC情况等。

jhat常用的选项包括：

-gc：打印Java堆的GC信息。

-port：指定服务器监听的端口号。

-XX:MaxHeapSize：指定Java进程的最大堆空间大小。

-XX:+HeapDumpOnOutOfMemoryError：在Java进程OOM时自动生成Java堆信息文件。

-XX:HeapDumpPath：指定Java堆信息文件的输出路径。

总之，jhat是一个方便且易于使用的Java堆分析工具，可以帮助开发人员更好地理解和调试Java程序的内存问题。 

## tldr 
 
> Java 堆分析工具。
> 更多信息：<https://docs.oracle.com/javase/8/docs/technotes/tools/unix/jhat.html>.

- 分析堆转储文件（来自 jmap），通过 http 端口 7000 进行查看：

`jhat {{路径/堆转储文件}}`

- 分析堆转储文件，为 http 服务指定备用端口：

`jhat -p {{端口}} {{路径/堆转储文件}}`

- 通过 jhat 分析转储文件，指定使用 8GB RAM（建议使用 2-4 倍的转储大小）：

`jhat -J-mx8G {{路径/堆转储文件}}`
