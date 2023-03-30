# go get 
## chatgpt 
The `go get` command in the Go programming language is used to download, build, and install packages and dependencies from version control repositories. It can be used to download and install packages from various hosting services, including GitHub, Bitbucket, and others.

When you execute the `go get` command followed by the package name, Go searches for the package in various repositories and downloads it to your `GOPATH` directory. It also downloads any dependencies required by the package and installs them in the `GOPATH` directory.

The basic syntax of the `go get` command is:

```
go get [flags] [package/path]
```

Here, `flags` are optional command-line options that modify the behavior of the command, and `package/path` is the path of the package or dependency you want to download.

Some common flags used with the `go get` command are:

- `-u` to update the package to the latest version
- `-v` to enable verbose output
- `-t` to download and install test dependencies

For example, to download and install the `"github.com/gorilla/mux"` package, you can execute the following command:

```
go get github.com/gorilla/mux
```

This command will download the package and its dependencies to your `GOPATH` directory, allowing you to use it in your Go programs. 

## tldr 
 
> Add a dependency package, or download packages in legacy GOPATH mode.
> More information: <https://pkg.go.dev/cmd/go#hdr-Add_dependencies_to_current_module_and_install_them>.

- Add a specified package to `go.mod` in module-mode or install the package in GOPATH-mode:

`go get {{example.com/pkg}}`

- Modify the package with a given version in module-aware mode:

`go get {{example.com/pkg}}@{{v1.2.3}}`

- Remove a specified package:

`go get {{example.com/pkg}}@{{none}}`
