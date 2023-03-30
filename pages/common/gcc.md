# gcc 
## chatgpt 
gcc stands for GNU Compiler Collection. It is a command-line compiler used to compile programs written in C, C++, and Objective-C programming languages. It is a popular compiler used in Linux and other Unix-based operating systems.

The gcc command is used to compile the source code of a program into an executable program that can be run on a computer. The basic format of the gcc command is:

gcc [options] filename

The options are various flags and settings that can be used to specify how the code is compiled, such as optimization level, output file name, and debugging information.

The filename should be the name of the main source file of the program. If there are multiple source files, they can be specified with additional filenames.

For example, to compile a C program called "hello.c", the command would be:

gcc -o hello hello.c

This command would create an executable program called "hello" from the source code in "hello.c". The "-o" option specifies the name of the output file.

Overall, gcc is a powerful tool used to compile and build programs in a variety of programming languages. 

## tldr 
 
> Preprocess and compile C and C++ source files, then assemble and link them together.
> More information: <https://gcc.gnu.org>.

- Compile multiple source files into an executable:

`gcc {{path/to/source1.c path/to/source2.c ...}} -o {{path/to/output_executable}}`

- Show common warnings, debug symbols in output, and optimize without affecting debugging:

`gcc {{path/to/source.c}} -Wall -g -Og -o {{path/to/output_executable}}`

- Include libraries from a different path:

`gcc {{path/to/source.c}} -o {{path/to/output_executable}} -I{{path/to/header}} -L{{path/to/library}} -l{{library_name}}`

- Compile source code into Assembler instructions:

`gcc -S {{path/to/source.c}}`

- Compile source code into an object file without linking:

`gcc -c {{path/to/source.c}}`
