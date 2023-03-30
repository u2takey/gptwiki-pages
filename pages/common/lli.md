# lli 
## chatgpt 
The command "lli" is an interpreter for LLVM Bitcode files. It runs programs that have been compiled to LLVM Bitcode format, rather than executable machine code. The "lli" command is part of the LLVM (Low Level Virtual Machine) toolchain, which is a collection of modular and reusable compiler and toolchain technologies designed to be embedded into a variety of programming languages and application frameworks.

The "lli" command is used to execute LLVM Bitcode programs directly and can be run in a terminal or command prompt window. It has several options, such as "-version" to display the version of LLVM, "-load" to load a dynamic library or plugin, and "-jit-kind" to specify the just-in-time (JIT) compiler to use.

One of the advantages of using "lli" is that it allows developers to rapidly test and debug their code without the need to compile to native binary code. Additionally, "lli" provides a powerful mechanism for dynamic profiling and optimization, allowing developers to track and analyze the performance of their programs at runtime.

In summary, the "lli" command is a powerful tool that allows developers to execute LLVM Bitcode programs directly, providing fast testing and debugging, dynamic profiling, and optimization capabilities. 

## tldr 
 
> Directly execute programs from LLVM bitcode.
> More information: <https://www.llvm.org/docs/CommandGuide/lli.html>.

- Execute a bitcode or IR file:

`lli {{path/to/file.ll}}`

- Execute with command line arguments:

`lli {{path/to/file.ll}} {{argument1 argument2 ...}}`

- Enable all optimizations:

`lli -O3 {{path/to/file.ll}}`

- Load a dynamic library before linking:

`lli --dlopen={{path/to/library.dll}} {{path/to/file.ll}}`
