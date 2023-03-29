# llvm-objdump 
## chatgpt 
llvm-objdump是一个用于反汇编和分析目标文件的命令行工具。它可以将编译后的可执行文件反编译为汇编代码，并且可以输出汇编代码的符号表、重定位信息等内容。

使用方式：

```
llvm-objdump [options] <object-file(s)>
```

其中，object-file是要分析的目标文件，可以是可执行文件、静态库、共享库等。

常用选项：

- -S：将原始的汇编代码与反汇编代码交替输出，以方便阅读和分析。
- -r：输出重定位信息。
- -t：输出符号表信息。
- -d：输出反汇编后的汇编代码。
- -j section-name：指定对某个节(section)进行反汇编。

示例：

下面是一个示例，展示如何使用llvm-objdump来查看一个可执行文件的汇编代码和符号表信息。

```
$ llvm-objdump -S -t ./a.out

./a.out：文件格式 Mach-O 64-bit executable x86_64

SYMBOL TABLE:
0000000100000000 g	 F	 .text	0000000000000069 _main
0000000100003f60 g	 __TEXT,__text	0000000000000000 _popcount
0000000100000000 g	 __TEXT,__text	0000000000000000 start
0000000100003ed0 g	 __DATA,__const	0000000000000004 _GREETER
0000000100000000        	__TEXT,__text	0000000000000000 __mh_execute_header
0000000100003f60        	__TEXT,__text	0000000000000000 __popcount

Disassembly of section __TEXT,__text:

0000000100000000 <start>:
   100000000:   55                      push   %rbp
   100000001:   48 89 e5                mov    %rsp,%rbp
   100000004:   c7 05 00 00 00 00 04    movl   $0x4,0x0(%rip)        # 10000000a <_main+0xa>
   10000000b:   00 00 00 
   ...
```

在上面的示例中，我们使用了-S和-t选项来输出了可执行文件a.out的符号表和反汇编代码。在符号表中，我们可以看到了目标文件中的一些符号，例如函数_main、常量_GREETER等。在反汇编代码中，我们可以看到了整个程序的汇编代码，以及每个汇编指令的地址和操作码。 

## tldr 
 
> 这是 `objdump` 命令的一个别名。

- 原命令的文档在：

`tldr objdump`
