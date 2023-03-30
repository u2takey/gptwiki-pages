# clangd 
## chatgpt 
`clangd` is a language server for C++ that provides IDE features such as code completion, go-to-definition, and refactoring. It uses the Clang C++ parser to analyze code and provides its functionality through a Language Server Protocol (LSP) which can be used by various IDEs and text editors. 

To use `clangd`, you typically need to install it first, after which you can use it from the command-line or from within an IDE or editor that supports LSP. 

The general syntax for using `clangd` from the command-line is: 

```
clangd [options] [file-or-directory]
```

Here, `[options]` refers to any optional command-line arguments that you can pass to `clangd` to customize its behavior. These include things like `-j` to specify the number of threads to use, `-log` to specify a log file, and so on.

`[file-or-directory]` refers to the path to a file or directory that contains the code you want to analyze. If you specify a file, `clangd` analyzes just that file. If you specify a directory, `clangd` recursively analyzes all files in the directory and its subdirectories.

Once you run `clangd`, it generates an index of your codebase, which it uses to provide its IDE-like features. You can then use an LSP-capable IDE/editor to connect to the `clangd` server and start using its features. 

## tldr 
 
> Language server that provides IDE-like features to editors.
> It should be used via an editor plugin rather than invoked directly.
> More information: <https://clangd.llvm.org/>.

- Display available options:

`clangd --help`

- List of available options:

`clangd --help-list`

- Display version:

`clangd --version`
