# xetex 
## chatgpt 
The `xetex` command is a command-line tool for typesetting documents using the XeTeX engine. XeTeX is a typesetting engine based on the TeX typesetting system that includes support for Unicode and modern font technologies like OpenType and Apple Advanced Typography. 

When you use the `xetex` command, it takes a TeX input file (usually with a `.tex` file extension) as its argument and processes it to create output files (such as a PDF or DVI file, depending on the options used). 

Some useful options that can be used with `xetex` include:

- `-pdf`: Generate a PDF output file directly
- `-output-driver=xdvipdfmx`: Set the output driver to XDVIPDFMX, which produces PDF output more quickly than the default driver (DVIPS)
- `-halt-on-error`: Stop processing the input file if an error is encountered
- `-shell-escape`: Allow the input file to execute shell commands 

In general, using the `xetex` command requires some familiarity with the TeX syntax and formatting rules. It is often used in conjunction with a text editor or integrated development environment that provides additional features like syntax highlighting, autocomplete, and error checking. 

## tldr 
 
> Compile a PDF document from XeTeX source files.
> More information: <https://www.tug.org/xetex/>.

- Compile a PDF document:

`xetex {{source.tex}}`

- Compile a PDF document, specifying an output directory:

`xetex -output-directory={{path/to/directory}} {{source.tex}}`

- Compile a PDF document, exiting if errors occur:

`xetex -halt-on-error {{source.tex}}`
