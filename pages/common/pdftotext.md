# pdftotext 
## chatgpt 
`pdftotext` is a command-line utility tool for converting PDF files to plain text files. Here’s the syntax of the command:

`pdftotext [options] [PDF-file] [output-file]`

The command can be executed on Windows, macOS, and Linux operating systems. Here’s how the command works:

1. When the command is executed, it looks for the `pdftotext` executable file on the system.

2. The command takes the PDF file that is to be converted and converts it to a plain text file.

3. The output file contains the text extracted from the PDF file.

4. The command takes options as inputs to customize the conversion process. Some of the commonly used options are:

   - `-layout` : The option preserves the original layout of the PDF file while converting it to plain text. 
   
   - `-nopgbrk` : The option removes the page breaks in the plain text file generated. 
   
   - `-enc` : The option specifies the encoding technique for the plain text file such as UTF-8, ASCII or UTF-16. 

5. The command outputs any error messages or status updates to the terminal.

In summary, `pdftotext` is a powerful tool for converting PDF files to plain text files with many customizable options available for the users to choose from. 

## tldr 
 
> Convert PDF files to plain text format.
> More information: <https://www.xpdfreader.com/pdftotext-man.html>.

- Convert `filename.pdf` to plain text and print it to standard output:

`pdftotext {{filename.pdf}} -`

- Convert `filename.pdf` to plain text and save it as `filename.txt`:

`pdftotext {{filename.pdf}}`

- Convert `filename.pdf` to plain text and preserve the layout:

`pdftotext -layout {{filename.pdf}}`

- Convert `input.pdf` to plain text and save it as `output.txt`:

`pdftotext {{input.pdf}} {{output.txt}}`

- Convert pages 2, 3 and 4 of `input.pdf` to plain text and save them as `output.txt`:

`pdftotext -f {{2}} -l {{4}} {{input.pdf}} {{output.txt}}`
