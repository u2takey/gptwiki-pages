# latexmk 
## chatgpt 
LaTeXmk is a command-line tool used to automate the process of compiling (or typesetting) LaTeX documents. It works by monitoring changes to the document files (e.g., the .tex file, any included .bib or .sty files, etc.) and automatically recompiling the document whenever necessary (e.g., if the source file has been modified).

The basic syntax of the latexmk command is as follows:

    latexmk [options] [filename(s)]

where [filename(s)] is the name of the main LaTeX document file (without the .tex extension) and [options] are various command-line options that can be used to customize the behavior of latexmk.

Some common options include:

- -pdf: Generate a PDF output file instead of a DVI file.
- -pvc: "Preview continuously" mode, where latexmk continuously monitors the source files and recompiles the document whenever necessary, updating the preview pane in a PDF viewer at the same time.
- -quiet: Suppress all output except for error messages.
- -gg: Generate a debug log file.

Latexmk can also be customized using a configuration file, which is typically named .latexmkrc and resides in the user's home directory.

Overall, the latexmk command is an invaluable tool for LaTeX users who want to streamline their workflow and spend less time manually recompiling their documents. 

## tldr 
 
> Compile LaTeX source files into finished documents.
> Automatically does multiple runs when needed.
> More information: <https://mg.readthedocs.io/latexmk.html>.

- Compile a DVI (Device Independent file) document from every source:

`latexmk`

- Compile a DVI document from a specific source file:

`latexmk {{source.tex}}`

- Compile a PDF document:

`latexmk -pdf {{source.tex}}`

- Force the generation of a document even if there are errors:

`latexmk -f {{source.tex}}`

- Clean up temporary TEX files created for a specific TEX file:

`latexmk -c {{source.tex}}`

- Clean up all temporary TEX files in the current directory:

`latexmk -c`
