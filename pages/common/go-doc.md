# go doc 
## chatgpt 
The `go doc` command is used in Go programming language to display the documentation of Go packages, functions, types, and methods. It provides a quick and easy way for developers to access documentation for Go code without leaving the command line environment.

Here's how the `go doc` command works:

1. First, the command is executed with the name of the package, function, or type you want to view the documentation for.

2. The command searches for the documentation associated with the item you specified, either in local documentation files or online.

3. If found, the documentation is displayed in your terminal window. You can scroll through the documentation using your keyboard's arrows or the "page up" and "page down" keys.

4. You can also use some optional flags with the `go doc` command to customize the output. For example, `go doc -cmd pkg` will display the documentation for a command package, while `go doc -all pkg` will display the documentation for all packages.

Overall, the `go doc` command is a powerful tool for Go developers, helping them quickly access and review documentation for their code without leaving the terminal environment. 

## tldr 
 
> Show documentation for a package or symbol.
> More information: <https://golang.org/cmd/go/#hdr-Show_documentation_for_package_or_symbol>.

- Show documentation for the current package:

`go doc`

- Show package documentation and exported symbols:

`go doc {{encoding/json}}`

- Show also documentation of symbols:

`go doc -all {{encoding/json}}`

- Show also sources:

`go doc -all -src {{encoding/json}}`

- Show a specific symbol:

`go doc -all -src {{encoding/json.Number}}`
