# tex 
## chatgpt 
The command "tex" is a command line program used to process TeX files, which are commonly used for typesetting documents such as research papers, reports, and books. When executed, the "tex" command reads a TeX file and generates an output file (usually a PDF) that contains the formatted content.

To use the "tex" command, you need to open a terminal/command prompt on your computer and navigate to the directory where the TeX file is located. Once you are in the correct directory, you can execute the "tex" command by typing "tex file.tex"(replace "file" with the name of your TeX file).

When the "tex" command is executed, it reads the TeX file and generates a "DVI" (Device Independent) output file, which is a format that can be used by other programs to generate various output formats, such as PDF or PostScript. To convert the DVI file to a PDF file, you can use another command-line tool called "dvipdf".

The "tex" command has many options that can be used to customize the typesetting process, such as specifying the font size or setting margins. These options are specified as command-line arguments when executing the "tex" command.

Overall, the "tex" command is a powerful tool for typesetting documents and is widely used in academic and technical fields for creating complex documents with precise formatting. 

## tldr 
 
> Compile a DVI document from TeX source files.
> More information: <https://www.tug.org/begin.html>.

- Compile a DVI document:

`tex {{source.tex}}`

- Compile a DVI document, specifying an output directory:

`tex -output-directory={{path/to/directory}} {{source.tex}}`

- Compile a DVI document, exiting on each error:

`tex -halt-on-error {{source.tex}}`
