# dmesg 
## chatgpt 
dmesg是一个用于显示系统启动信息的命令。它读取内核缓冲区（kernel ring buffer）中的信息，并以人类可读的形式输出到控制台（终端）中。dmesg命令通常用于调试和排查系统问题，也可以用于检查硬件设备是否正确识别或驱动程序是否正确加载。

dmesg命令的输出内容通常包括系统启动信息、设备信息、内核模块的加载和卸载信息等内容。其中，系统启动信息包括引导加载程序（bootloader）启动内核的过程，系统硬件初始化的过程等信息；设备信息包括系统中存在的设备编号、设备名称、设备类型等等；内核模块信息包括内核模块的加载和卸载信息，以及模块间的依赖关系和参数等信息。通过dmesg命令可以查看内核缓冲区中的所有信息，也可以使用grep等命令筛选特定信息。

举例来说，如果想查看所有包含“error”或“warning”的信息，可以使用以下命令：

dmesg | grep -E 'error|warning'

这将输出所有包含“error”或“warning”的信息。使用dmesg命令还可以将输出信息写入文件中，供后续分析使用。例如：

dmesg > dmesg_output.txt

这将把dmesg输出信息写入到名为dmesg_output.txt的文件中。 

## tldr 
 
> 将内核消息写入标准输出。
> 更多信息：<https://www.manpagez.com/man/8/dmesg/>.

- 显示内核消息：

`dmesg`

- 显示此系统上有多少可用的物理内存：

`dmesg | grep -i memory`

- 一次显示一页内核消息：

`dmesg | less`
