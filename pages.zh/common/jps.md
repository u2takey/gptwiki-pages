# jps 
## chatgpt 
jps是Java Virtual Machine Process Status Tool的缩写，是一个用于查看Java虚拟机（JVM）上运行进程的命令行工具。简单来说，它可以帮助您在命令行中查看当前在运行的Java应用程序和它们的进程ID。

使用jps命令，您可以了解Java应用程序的状态和运行信息，例如应用程序的名称、进程ID、应用程序主类等。此外，您还可以使用jps命令来确定某个应用程序是否在运行中。

以下是jps命令的一些常见选项：

- -q：只输出进程ID，不输出进程名称。
- -m：输出进程的参数信息。
- -l：输出进程的完整类名。
- -v：输出进程的JVM参数信息。
- -V：输出jps程序的版本信息。

总之，jps命令是一个非常有用的工具，可以帮助您快速了解Java应用程序的状态、运行信息等。它在调试和监控Java程序时非常有用。 

## tldr 
 
> 显示当前用户的 JVM 进程状态。
> 更多信息：<https://docs.oracle.com/en/java/javase/11/tools/jps.html>.

- 列出所有 JVM 进程：

`jps`

- 列出所有 JVM 进程，只打印进程号：

`jps -q`

- 显示传递给进程的参数：

`jps -m`

- 显示所有进程的完整软件包名称：

`jps -l`

- 显示传递给 JVM 的参数：

`jps -v`
