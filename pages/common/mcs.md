# mcs 
## chatgpt 
The command "mcs" is used in the Mono development platform for compiling C# code. It is an abbreviation for "Mono C# Compiler". The command is used to generate an executable file from C# source code or to create a dynamic link library (DLL) from C# code. The syntax for the "mcs" command varies depending on the operating system being used.

For example, on Linux or macOS, the basic syntax for the mcs command is:

mcs [options] [source files]

Here, options refer to command-line arguments used to set various compiler options such as defining constants, setting warning levels, specifying the output file name, and so on. One or more source files must be specified as arguments.

On Windows, the syntax for the "mcs" command is slightly different:

mcs.exe [options] [source files]

The "mcs" command can be used to compile C# code into standalone executables or dynamic-link libraries (DLLs). It is one of the key components of the Mono development platform, which is an open-source alternative to Microsoft's .NET Framework. It allows developers to write C# code that can run on any platform that supports Mono, including Linux, macOS, and Windows. 

## tldr 
 
> Mono C# Compiler.
> More information: <https://manned.org/mcs.1>.

- Compile the specified files:

`mcs {{path/to/input_file1.cs path/to/input_file2.cs ...}}`

- Specify the output program name:

`mcs -out:{{path/to/file.exe}} {{path/to/input_file1.cs path/to/input_file2.cs ...}}`

- Specify the output program type:

`mcs -target:{{exe|winexe|library|module}} {{path/to/input_file1.cs path/to/input_file2.cs ...}}`
