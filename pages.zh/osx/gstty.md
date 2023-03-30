# gstty 
## chatgpt 
gstty是一个实用程序命令，用于设置终端的模式参数和特殊字符处理功能。它的作用是控制终端的行为，比如说回显和字符映射等。具体的命令参数可以通过gstty --help命令来查看。

一些常用的gstty命令参数：

- -a或--all：显示所有设置参数以及相应的意义；
- -echo或-echoe或-echoctl或-echoprt或-echoke：控制回显的方式；
- -icanon或-cbreak：控制行缓冲的方式；
- -isig或-ignbrk或-ignpar或-tostop：控制输入和输出的信号，以及输出方式；
- -time或-min或-sw0或-sw2：控制输入的等待时间和终端处理行为。

例如，gstty -a命令可以显示当前终端的所有设置参数，而gstty -echo可以关闭回显功能。 

## tldr 
 
> 这是 `-p linux stty` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux stty`
