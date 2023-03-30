# brittany 
## chatgpt 
As an AI language model, I can tell you that "brittany" is not a command; rather, it can refer to several entities such as a region in France, a female given name, or a software tool named Brittany that is used for cleaning up and formatting Haskell code. 

Assuming that you are referring to the software tool, "Brittany" is typically used in command line interfaces to format Haskell source code. The basic command syntax is as follows:

`brittany [OPTIONS] [FILES]`

Here, `[OPTIONS]` refers to any additional flags or options for the command, while `[FILES]` are the source code files that need to be formatted. For example, to format a single file, you can use the command:

`brittany MyModule.hs`

To format all `.hs` files in a directory and its subdirectories, you can use the recursive flag `-r`:

`brittany -r *.hs`

Some other commonly used options include:

- `--write-mode`: Specify whether the formatted code should be written to a file or printed to the console.
- `--indent`: Specify the number of spaces to use for indentation.
- `--columns`: Specify the maximum line width for the formatted code.

Note that before using Brittany, you need to install it on your computer. The installation instructions may vary depending on your operating system and package manager, but typically involve running a command like:

`cabal install brittany`

or

`stack install brittany`

Once installed, you can use the `brittany` command in your terminal or command prompt to format Haskell code according to your preferred style guide. 

## tldr 
 
> Pretty-print Haskell source files.
> More information: <https://github.com/lspitzner/brittany#readme>.

- Format a Haskell source file and print the result to `stdout`:

`brittany {{path/to/file.hs}}`

- Format all Haskell source files in the current directory in-place:

`brittany --write-mode=inplace {{*.hs}}`

- Check whether a Haskell source file needs changes and indicate the result through the programme's exit code:

`brittany --check-mode {{path/to/file.hs}}`

- Format a Haskell source file using the specified amount of spaces per indentation level and line length:

`brittany --indent {{4}} --columns {{100}} {{path/to/file.hs}}`

- Format a Haskell source file according to the style defined in the specified config file:

`brittany --config-file {{path/to/config.yaml}} {{path/to/file.hs}}`
