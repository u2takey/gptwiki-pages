# gprbuild 
## chatgpt 
gprbuild is a command used to build Ada programs or components. It is part of the GNAT Ada Development Environment (GNAT) suite of tools, which is the GNU implementation of the Ada programming language.

The command is executed from the command line, and it builds a project file. The project file is a text file that describes the structure and dependencies of the Ada program or component being built. The project file has the extension ".gpr".

When executed, gprbuild reads the project file and compiles the source code files listed in it. It also links the compiled object files into an executable or a library, depending on the configuration specified in the project file.

The gprbuild command also supports many command-line options to customize the build process. Some of the most commonly used options include:

- -P: specifies the project file to use
- -X: specifies the name and value of a project variable
- -j: specifies the number of parallel jobs to use for compilation and linking
- -gnatwa: specifies the level of warnings to display during compilation

Overall, the gprbuild command is a powerful tool for building Ada programs and components. Its use of project files and customizable options make it flexible and adaptable to a wide range of build configurations. 

## tldr 
 
> A high-level build tool for projects written in Ada and other languages (C/C++/Fortran).
> More information: <https://docs.adacore.com/gprbuild-docs/html/gprbuild_ug.html>.

- Build a project (assuming only one `*.gpr` file exists in the current directory):

`gprbuild`

- Build a specific [P]roject file:

`gprbuild -P{{project_name}}`

- Clean up the build workspace:

`gprclean`

- Install compiled binaries:

`gprinstall --prefix {{path/to/installation/dir}}`
