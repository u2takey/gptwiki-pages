# lualatex 
## chatgpt 
lualatex is a command used to compile LaTeX files that contain Lua code. Lua is a light-weight and efficient scripting language that can be used in conjunction with LaTeX to create dynamic and interactive documents.

When the lualatex command is invoked, it processes the input LaTeX file and compiles it into a PDF document. The command first parses the input file and processes all the LaTeX commands, as the standard pdflatex command does. However, if the input file contains Lua code, lualatex will also process this code and execute it during the compilation process.

Lualatex provides several advantages over other LaTeX compilers. First, it allows for the direct embedding of Lua code in LaTeX documents, enabling you to create more advanced and interactive documents. Additionally, lualatex has better Unicode support, allowing for higher-quality output that can handle non-Latin character sets.

Overall, lualatex is an invaluable tool for LaTeX users who want to create more advanced and interactive documents with the use of Lua code. 

## tldr 
 
> An extended version of TeX using Lua to compile.
> More information: <https://manned.org/lualatex.1>.

- Start `texlua` to act as a Lua interpreter:

`lualatex`

- Compile a Tex file to PDF:

`lualatex {{path/to/file.tex}}`

- Compile a Tex file without error interruption:

`lualatex -interaction nonstopmode {{path/to/file.tex}}`

- Compile a Tex file with a specific output file name:

`lualatex -jobname={{filename}} {{path/to/file.tex}}`
