# pandoc 
## chatgpt 
The command "pandoc" is a command-line tool for converting documents from one format to another. It was developed by John MacFarlane in 2006 and is now a popular tool used by many writers and publishers.

Pandoc supports over 40 input and output document formats, including Markdown, HTML, LaTeX, Microsoft Word, and PDF. It can convert between these formats, allowing writers to create content in a format that suits their workflow and then convert it to the desired output format for publication.

To use the command, you will need to have Pandoc installed on your computer. Once installed, you can open a terminal or command prompt and enter the "pandoc" command along with any necessary options and arguments. For example, to convert a Markdown file to HTML, you could enter the following command:

```
pandoc input.md -o output.html
```

In this command, "input.md" is the file you want to convert, and "-o output.html" specifies the output file name and format. Pandoc will then convert the Markdown file to HTML and save it in the specified output file.

Pandoc has many other options and features that allow you to customize the conversion process, such as specifying fonts and styles for PDF output, adding metadata to your documents, and including table of contents and references. You can find more information on using Pandoc in the official documentation. 

## tldr 
 
> Convert documents between various formats.
> More information: <https://pandoc.org>.

- Convert file to PDF (the output format is determined by file extension):

`pandoc {{input.md}} -o {{output.pdf}}`

- Force conversion to use a specific format:

`pandoc {{input.docx}} --to {{gfm}} -o {{output.md}}`

- Convert to a standalone file with the appropriate headers/footers (for LaTeX, HTML, etc.):

`pandoc {{input.md}} -s -o {{output.tex}}`

- List all supported input formats:

`pandoc --list-input-formats`

- List all supported output formats:

`pandoc --list-output-formats`
