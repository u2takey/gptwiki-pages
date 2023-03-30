# cppclean 
## chatgpt 
`cppclean` is a command-line tool used for analyzing C++ source code and identifying potential issues related to code quality, maintainability, and style. The tool scans the source code files and detects various problems and inefficiencies in the code that could lead to bugs, crashes, and other issues. 

Some of the issues that `cppclean` identifies are:
- Unused code
- Duplicate code
- Code that violates coding style guidelines
- Memory leaks
- Uninitialized variables
- Undefined behavior
- Type mismatches

The `cppclean` tool uses static analysis techniques to perform these checks, without the need for compiling or running the code. It generates a report of the identified issues, along with recommendations for fixing them.

The basic syntax for running `cppclean` is:
```
cppclean [options] <directory or file>
```

Here, `options` are various command-line options that can be used to customize the analysis process or output format. The `<directory or file>` argument specifies the location of the C++ source code to be analyzed.

The `cppclean` tool is platform-independent and can be used on Windows, Linux, and macOS systems. 

## tldr 
 
> Find unused code in C++ projects.
> More information: <https://github.com/myint/cppclean>.

- Run in a project's directory:

`cppclean {{path/to/project}}`

- Run on a project where the headers are in the `inc1/` and `inc2/` directories:

`cppclean {{path/to/project}} --include-path={{inc1}} --include-path={{inc2}}`

- Run on a specific file `main.cpp`:

`cppclean {{main.cpp}}`

- Run on the current directory, excluding the "build" directory:

`cppclean {{.}} --exclude={{build}}`
