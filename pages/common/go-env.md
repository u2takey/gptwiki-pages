# go env 
## chatgpt 
The command "go env" is used to display Go environment information in the terminal. This command is useful when developing Go applications to understand the current environment settings. 

When "go env" is executed, it prints a list of key-value pairs representing environment variables that are relevant to Go. These variables are used to configure Go runtime and toolchain behaviour. 

Some of the key-value pairs that are printed include:

- GOARCH: The target architecture (e.g. amd64, arm).
- GOBIN: The directory where Go executables are installed.
- GOCACHE: The directory where Go caches build and test results.
- GOOS: The target operating system (e.g. linux, windows).
- GOPATH: The workspace directory where Go source files are stored.
- GOROOT: The directory where the Go compiler and standard library are installed.

By default, "go env" prints all environment variables related to Go. However, you can use flags to print only specific variables of interest. For example, "go env GOPATH" would print the value of the GOPATH environment variable. 

## tldr 
 
> Manage environment variables used by the Go toolchain.
> More information: <https://golang.org/cmd/go/#hdr-Print_Go_environment_information>.

- Show all environment variables:

`go env`

- Show a specific environment variable:

`go env {{GOPATH}}`

- Set an environment variable to a value:

`go env -w {{GOBIN}}={{path/to/directory}}`

- Reset an environment variable's value:

`go env -u {{GOBIN}}`
