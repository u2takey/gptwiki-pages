# go 
## chatgpt 
The "go" command is a command-line tool used for managing Go source code. When the command "go" is executed in the command line, it can run several subcommands that may be useful for developers.

Some of the commonly used subcommands of "go" include "build," which compiles the program in the current directory and outputs the executable binary, "run," which compiles and runs the executable binary, "test," which runs the package tests and reports the results, and "install," which downloads, compiles, and installs packages and dependencies.

The "go" command also provides other commands for managing dependencies, including "get," "mod," and "vendor." Users can use "go get" to download packages and dependencies, "go mod" to manage module versions and requirements, and "go vendor" to create a local copy of the code and its dependencies for offline use.

Overall, the "go" command provides a convenient way to manage Go projects and packages, from building the executable binary to managing dependencies. 

## tldr 
 
> Tool for managing go source code.
> Some subcommands such as `go build` have their own usage documentation.
> More information: <https://golang.org>.

- Download and install a package, specified by its import path:

`go get {{package_path}}`

- Compile and run a source file (it has to contain a `main` package):

`go run {{file}}.go`

- Compile a source file into a named executable:

`go build -o {{executable}} {{file}}.go`

- Compile the package present in the current directory:

`go build`

- Execute all test cases of the current package (files have to end with `_test.go`):

`go test`

- Compile and install the current package:

`go install`

- Initialize a new module in the current directory:

`go mod init {{module_name}}`
