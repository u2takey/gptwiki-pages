# csc 
## chatgpt 
csc is a command line tool used to compile C# programs. CSC stands for "C# Compiler" and is used to create executable files of C# code. 

When used, the csc command will take in C# code files (.cs files) as input and compile them into executable files (.exe files). The command can also be used to compile multiple source files at once and can also create .dll files (Dynamic Link Libraries) from C# code.

The syntax for using the csc command is as follows:

csc [options] [sourcefiles]

The options refer to any additional options or switches used when compiling the code such as target framework, output path, or optimizations. The source files refer to the C# code files that need to be compiled into an executable or .dll file.

After the command is executed, the compiler will analyze, validate, and convert the C# code into an executable form, which can then be run on a compatible platform. Any errors or warnings encountered during the compilation process will be displayed in the command prompt. 

## tldr 
 
> The Microsoft C# Compiler.
> More information: <https://learn.microsoft.com/dotnet/csharp/language-reference/compiler-options/command-line-building-with-csc-exe>.

- Compile one or more C# files to a CIL executable:

`csc {{path/to/input_file_a.cs}} {{path/to/input_file_b.cs}}`

- Specify the output filename:

`csc /out:{{path/to/filename}} {{path/to/input_file.cs}}`

- Compile into a `.dll` library instead of an executable:

`csc /target:library {{path/to/input_file.cs}}`

- Reference another assembly:

`csc /reference:{{path/to/library.dll}} {{path/to/input_file.cs}}`

- Embed a resource:

`csc /resource:{{path/to/resource_file}} {{path/to/input_file.cs}}`

- Automatically generate XML documentation:

`csc /doc:{{path/to/output.xml}} {{path/to/input_file.cs}}`

- Specify an icon:

`csc /win32icon:{{path/to/icon.ico}} {{path/to/input_file.cs}}`

- Strongly-name the resulting assembly with a keyfile:

`csc /keyfile:{{path/to/keyfile}} {{path/to/input_file.cs}}`
