# pdflatex 
## chatgpt 
pdflatex is a command line tool for typesetting documents written in LaTeX language, a document preparation system used in academic and scientific fields. 

When executed, pdflatex will take a LaTeX document file (.tex) as input and compile it to produce a PDF document (.pdf). During this process, pdflatex parses the LaTeX code, processes the formatting and typesetting instructions, and generates the output PDF file.

The command pdflatex can be run from a terminal or command prompt with the following syntax:

```
pdflatex [options] filename.tex
```

The filename.tex argument specifies the name of the LaTeX document to be processed. The options parameter can be used to customize the behavior of pdflatex, such as specifying output directories, enabling or disabling certain features or packages, and adjusting the verbosity of the output produced during the compilation process.

Here are some commonly used options for pdflatex:

- `-output-directory` specifies the directory where the output (PDF) file should be saved
- `-halt-on-error` terminates the compilation process if an error occurs
- `-synctex` generates a file that allows for synchronization between the LaTeX source code and the generated PDF output, enabling easy navigation between the two
- `-interaction` determines the level of interaction desired during the compilation process, with the following options:
  - `nonstopmode` runs the compilation without stopping for input, useful for batch processing
  - `scrollmode` runs the compilation without stopping, but displaying output on the screen as it happens
  - `errorstopmode` pauses the compilation upon encountering errors, waiting for user input to continue or terminate the process

Overall, pdflatex is an essential tool for anyone working with LaTeX documents, allowing for the creation of high-quality typeset documents in a variety of academic and scientific fields. 

## tldr 
 
> Compile a PDF document from LaTeX source files.
> More information: <https://manned.org/pdflatex>.

- Compile a PDF document:

`pdflatex {{source.tex}}`

- Compile a PDF document specifying an output directory:

`pdflatex -output-directory={{path/to/directory}} {{source.tex}}`

- Compile a PDF document, exiting on each error:

`pdflatex -halt-on-error {{source.tex}}`
