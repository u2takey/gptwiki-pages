# adscript 
## chatgpt 
我很抱歉，我无法详细解释adscript命令，因为无法确定这是哪个操作系统或程序中的命令。 请提供更多上下文，例如操作系统或程序名称，以便我能够提供更加准确的解释。 

## tldr 
 
> 用于 Adscript 文件的编译器。
> 更多信息：<https://github.com/Amplus2/Adscript>.

- 将一个文件编译为一个对象文件：

`adscript --output {{路径/到/文件.o}} {{路径/到/输入文件.adscript}}`

- 编译并链接一个文件到一个独立的可执行文件：

`adscript --executable --output {{路径/到/文件}} {{路径/到/输入文件.adscript}}`

- 将文件编译成 LLVM IR 而不是本地机器码：

`adscript --llvm-ir --output {{路径/到/文件.ll}} {{路径/到/输入文件.adscript}}`

- 将一个文件交叉编译为一个其他 CPU 架构或操作系统的目标文件：

`adscript --target-triple {{i386-linux-elf}} --output {{路径/到/文件.o}} {{路径/到/输入文件.adscript}}`
