# g++ 
## chatgpt 
g++ is a command-line utility that is often used to compile C++ language code into executable binary files. The command is available on most Unix systems, including Linux and macOS.

When you execute the g++ command, you are telling your computer to invoke the GNU C++ compiler. You usually include the name of the source file to be compiled as an argument in the command. For instance, if you have a file named main.cpp which contains C++ source code, the command to compile that file using g++ will usually look like this:

$ g++ main.cpp -o output_file

The -o option specifies the name of the output file. In this example, the compiled executable file will be named output_file.

The g++ command-line utility has many other options that you can use to customize the compilation process, such as:

- -c: Compile source files into object files without linking them into an executable file
- -g: Include debugging information in the compiled code
- -Wall: Enable all compiler warnings
- -O: Optimize the compiled code for performance

Overall, the g++ command is a powerful tool for compiling C++ code and creating executable files for a variety of platforms. 

## tldr 
 
> Compiles C++ source files.
> Part of GCC (GNU Compiler Collection).
> More information: <https://gcc.gnu.org>.

- Compile a source code file into an executable binary:

`g++ {{path/to/source.cpp}} -o {{path/to/output_executable}}`

- Display common warnings:

`g++ {{path/to/source.cpp}} -Wall -o {{path/to/output_executable}}`

- Choose a language standard to compile for (C++98/C++11/C++14/C++17):

`g++ {{path/to/source.cpp}} -std={{c++98|c++11|c++14|c++17}} -o {{path/to/output_executable}}`

- Include libraries located at a different path than the source file:

`g++ {{path/to/source.cpp}} -o {{path/to/output_executable}} -I{{path/to/header}} -L{{path/to/library}} -l{{library_name}}`

- Compile and link multiple source code files into an executable binary:

`g++ -c {{path/to/source_1.cpp path/to/source_2.cpp ...}} && g++ -o {{path/to/output_executable}} {{path/to/source_1.o path/to/source_2.o ...}}`

- Display version:

`g++ --version`
