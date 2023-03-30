# llvm-config 
## chatgpt 
`llvm-config` is a command-line utility that is used to retrieve various configuration options and system information about the LLVM compiler infrastructure. It can be used to query for information about LLVM in order to aid in the development or use of LLVM-based software.

Some of the important options that can be retrieved using the `llvm-config` command include:

1. `--version`: This option prints the version number of LLVM that is currently installed on the system.
2. `--cppflags`: This option retrieves the C++ compiler flags that are required to build software that uses LLVM. This includes include paths and other options that are required to properly link against LLVM.
3. `--ldflags`: This option retrieves the linker flags that are required to link against LLVM libraries.
4. `--libs`: This option retrieves the names of the LLVM libraries that should be linked into a software project. This is typically used along with `--ldflags` to properly link against LLVM.
5. `--libdir`: This option retrieves the path to the directory that contains the LLVM libraries.

The `llvm-config` command is typically installed along with the LLVM compiler infrastructure and is available on most Unix-based operating systems, including Linux and macOS. 

## tldr 
 
> Get various configuration information needed to compile programs which use LLVM.
> Typically called from build systems, like in Makefiles or configure scripts.
> More information: <https://llvm.org/docs/CommandGuide/llvm-config.html>.

- Compile and link an LLVM based program:

`clang++ $(llvm-config --cxxflags --ldflags --libs) --output {{path/to/output_executable}} {{path/to/source.cc}}`

- Print the `PREFIX` of your LLVM installation:

`llvm-config --prefix`

- Print all targets supported by your LLVM build:

`llvm-config --targets-built`
