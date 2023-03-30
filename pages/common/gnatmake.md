# gnatmake 
## chatgpt 
The gnatmake command is a compiler driver that takes Ada source code files as input and produces executable programs as output. It is part of the GNAT Ada development environment, which includes a complete set of compilers, tools, and libraries for developing and testing Ada programs.

The gnatmake command simplifies the build process by automatically compiling and linking all the necessary source code files to create an executable program. It is also capable of generating dependency information to help automate the build process in the future.

The command takes one or more input files as arguments and produces an executable file with the same name as the first input file, but with an appropriate extension. For example, if the input file is named "program.adb", the output file will be named "program" on Unix-like systems and "program.exe" on Windows systems.

The gnatmake command also supports a variety of options to control the compilation and linking process, such as specifying optimization levels, debugging information, and library paths. The most commonly used options are "-c" to compile only (without linking), "-s" to show the commands executed, and "-jN" to specify the number of parallel compilations.

Overall, the gnatmake command is a powerful and flexible tool for building Ada programs, making it an essential component of any Ada development environment. 

## tldr 
 
> A low-level build tool for Ada programs (part of the GNAT toolchain).
> More information: <https://gcc.gnu.org/onlinedocs/gnat_ugn/Building-with-gnatmake.html>.

- Compile an executable:

`gnatmake {{source_file1.adb source_file2.adb ...}}`

- Set a custom executable name:

`gnatmake -o {{executable_name}} {{source_file.adb}}`

- [f]orce recompilation:

`gnatmake -f {{source_file.adb}}`
