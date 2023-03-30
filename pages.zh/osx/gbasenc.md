# gbasenc 
## chatgpt 
gbasenc是一个用于将GBA汇编文件编译成可执行二进制文件的命令。

该命令需要输入两个参数：

1. 源文件名：要编译的GBA汇编文件名称，必须以.asm为后缀。

2. 目标文件名：编译成功后生成的可执行二进制文件名，必须以.gba为后缀。

该命令会将汇编代码编译成GBA可执行二进制文件，并输出编译信息和警告。编译过程中，可以通过使用指令（如.equ）进行定义、使用标号等。在编译成功后，生成的可执行文件可以在GBA模拟器或实际的GBA游戏机上运行。

注意：使用gbasenc命令需要安装DevKitAdvance开发工具包，且需要在安装路径下使用命令行才能正常运行。 

## tldr 
 
> 这是 `-p linux basenc` 命令的一个别名。

- 原命令的文档在：

`tldr -p linux basenc`