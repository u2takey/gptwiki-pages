# go install 
## chatgpt 
The `go install` command is a command-line tool used in Go programming language to install and compile packages or software programs that are available in a Go repository.

When executed, the command compiles and installs the code in the package directory of the specified package into the bin directory of the Go workspace. The executable binary files are saved in the bin directory, and the Go packages are saved in the pkg directory.

This command is particularly useful for installing Go packages that can be used in other Go programs. For instance, if a developer wants to use a specific Go package in their program, they can use this command to install the package and compile it for use.

It is important to note that the command needs to be executed in the directory where the main Go file is located or in the package directory of the specified package. Additionally, the command should be executed with administrative or root privileges, especially when installing packages globally. 

## tldr 
 
> Compile and install packages named by the import paths.
> More information: <https://pkg.go.dev/cmd/go#hdr-Compile_and_install_packages_and_dependencies>.

- Compile and install the current package:

`go install`

- Compile and install a specific local package:

`go install {{path/to/package}}`

- Install the latest version of a program, ignoring `go.mod` in the current directory:

`go install {{golang.org/x/tools/gopls}}@{{latest}}`

- Install a program at the version selected by `go.mod` in the current directory:

`go install {{golang.org/x/tools/gopls}}`
