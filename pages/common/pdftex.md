# pdftex 
## chatgpt 
pdftex is a command-line program that is used to compile a LaTeX document into a PDF file. It is designed to be compatible with the standard LaTeX format and includes additional features for creating PDF documents, such as the ability to embed fonts and add hyperlinks.

To use pdftex, you need to have a LaTeX source file (typically a .tex file) that you want to compile. The basic syntax for using pdftex is:

```
pdftex filename.tex
```

This command will compile the LaTeX source file and produce a PDF output file with the same name as the input file (but with a .pdf extension).

The pdftex command supports a variety of options and settings that can be used to customize the output. Some common options include:

- -interaction: sets the level of interaction with the user during compilation (e.g., "nonstopmode" will suppress all output messages)
- -output-directory: specifies the directory where the output file should be written
- -synctex: enables the synchronization between source and output files for easier navigation

Overall, pdftex is a powerful tool for creating high-quality PDF documents from LaTeX source code. 

## tldr 
 
> Compile a PDF document from TeX source files.
> More information: <https://www.tug.org/applications/pdftex/>.

- Compile a PDF document:

`pdftex {{source.tex}}`

- Compile a PDF document, specifying an output directory:

`pdftex -output-directory={{path/to/directory}} {{source.tex}}`

- Compile a PDF document, exiting on each error:

`pdftex -halt-on-error {{source.tex}}`
