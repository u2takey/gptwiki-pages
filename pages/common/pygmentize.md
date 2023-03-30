# pygmentize 
## chatgpt 
Pygmentize is a command-line tool used to syntax highlight source code. It is a part of the Pygments library, which is a Python-based syntax highlighting tool.

When executed, pygmentize takes input from the standard input or a file and outputs the highlighted result to the standard output or a file. The output can be formatted in various styles like HTML, LaTeX, RTF, ANSI color escape sequences, etc.

Pygmentize supports a wide range of programming languages, markup languages, and document formats. It can detect the input language automatically, but you can also specify the language explicitly using the -l/--language option.

For example, to highlight a Python source code file named "hello.py" and output the result to an HTML file named "hello.html" using the "fruity" style, you can use the following command:

```
pygmentize -f html -O full,style=fruity hello.py > hello.html
```

Here, `-f html` specifies the output format as HTML, `-O full,style=fruity` specifies the output options (full means including line numbers and style=fruity defines the style to use), `hello.py` is the input file, and `> hello.html` redirects the output to the file named "hello.html".

Overall, pygmentize is a useful tool for developers and writers who need to share or publish source code in a more readable and attractive format. 

## tldr 
 
> Python-based syntax highlighter.
> More information: <https://pygments.org/docs/cmdline/>.

- Highlight file syntax and print to standard output (language is inferred from the file extension):

`pygmentize {{file.py}}`

- Explicitly set the language for syntax highlighting:

`pygmentize -l {{javascript}} {{input_file}}`

- List available lexers (processors for input languages):

`pygmentize -L lexers`

- Save output to a file in HTML format:

`pygmentize -f html -o {{output_file.html}} {{input_file.py}}`

- List available output formats:

`pygmentize -L formatters`

- Output an HTML file, with additional formatter options (full page, with line numbers):

`pygmentize -f html -O "full,linenos=True" -o {{output_file.html}} {{input_file}}`
