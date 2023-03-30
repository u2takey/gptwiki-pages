# go build 
## chatgpt 
`go build` is a command used in Go programming language to compile and build an executable binary file from the source code files. It is a tool that allows Go developers to create a standalone executable from their code.

When you run the `go build` command, the Go compiler reads the source code files in the current directory, and compiles them into an executable binary file. The resulting binary file can then be executed on any machine that has the same operating system and architecture as the one on which it was compiled.

Go build follows a few build constraints to create the executable file. These include:

- The Go build command follows the build constraints defined in the source code.
- It compiles only the package in the current directory, and any other packages that it imports.
- It does not compile tests, documentation, or other non-essential files.
- The resulting binary file is named the same as the package containing the main function.

The `go build` command can also take additional arguments to customize the build process, such as:

- `-o`: This flag specifies the name and path of the output file. By default, the output file is named after the package directory.
- `-v`: This flag increases the verbosity of the command to show more details about the build process.
- `-race`: This flag enables the race detector to detect data races in the program.
- `-tags`: This flag allows developers to specify build tags to include or exclude parts of the code when building.

Overall, go build is a crucial command that developers use often to compile their code into a standalone executable, making it easy to share, distribute, and run on other machines. 

## tldr 
 
> Compile Go sources.
> More information: <https://golang.org/cmd/go/#hdr-Compile_packages_and_dependencies>.

- Compile a 'package main' file (output will be the filename without extension):

`go build {{path/to/main.go}}`

- Compile, specifying the output filename:

`go build -o {{path/to/binary}} {{path/to/source.go}}`

- Compile a package:

`go build -o {{path/to/binary}} {{path/to/package}}`

- Compile a main package into an executable, enabling data race detection:

`go build -race -o {{path/to/executable}} {{path/to/main/package}}`
