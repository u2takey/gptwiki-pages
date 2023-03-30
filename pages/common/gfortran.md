# gfortran 
## chatgpt 
gfortran is a command-line compiler for the Fortran programming language. It is part of the GNU Compiler Collection (GCC) and is available for a variety of operating systems, including Linux, Mac OS, and Windows.

When executed, gfortran reads the Fortran source code files and compiles them into an executable binary file that can be run on the target platform. It also provides a number of options and flags that can be used to control the compilation process and optimize the resulting executable code.

Some of the key options and flags that can be used with gfortran include:

- -c: Compile the source code files into object files, but do not link them into an executable binary.
- -o: Specify the name of the output file (executable binary or object file).
- -Wall: Enable all warning messages.
- -O: Optimize the resulting code for speed.
- -g: Generate debug information for use with a debugger.
- -fPIC: Generate position-independent code (PIC) suitable for use in shared libraries.
- -static-libgfortran: Link the program statically to the libgfortran library.

Overall, gfortran is a powerful and flexible tool for compiling and optimizing Fortran code on a variety of platforms. 

## tldr 
 
> Preprocess and compile Fortran source files, then assemble and link them together.
> More information: <https://gcc.gnu.org/wiki/GFortran>.

- Compile multiple source files into an executable:

`gfortran {{path/to/source1.f90 path/to/source2.f90 ...}} -o {{path/to/output_executable}}`

- Show common warnings, debug symbols in output, and optimize without affecting debugging:

`gfortran {{path/to/source.f90}} -Wall -g -Og -o {{path/to/output_executable}}`

- Include libraries from a different path:

`gfortran {{path/to/source.f90}} -o {{path/to/output_executable}} -I{{path/to/mod_and_include}} -L{{path/to/library}} -l{{library_name}}`

- Compile source code into Assembler instructions:

`gfortran -S {{path/to/source.f90}}`

- Compile source code into an object file without linking:

`gfortran -c {{path/to/source.f90}}`
