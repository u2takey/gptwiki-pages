# tabula 
## chatgpt 
Tabula is a command-line tool that is used to extract tables from PDF files. It is an open-source Java application that allows users to quickly and easily extract data from PDF files that contain tables, which can then be saved in a variety of formats, including CSV, TSV, and HTML.

To use Tabula, you need to first download and install the software on your system. Once installed, the command "tabula" can be used to extract tables from PDF files. The basic syntax of the command is as follows:

tabula [OPTIONS] -f [FORMAT] -o [OUTPUT FILE] [INPUT FILE]

- [OPTIONS] – This is an optional argument that can be used to provide additional command-line options and arguments to the Tabula command. Some of the available options include specifying the page numbers of the PDF file to extract tables from, selecting a specific area of the page to extract data from, and specifying the delimiter to use when outputting data as CSV or TSV.

- -f [FORMAT] – This argument is used to specify the output format for the extracted table data. The available options include csv, tsv, html, and json. The default format is CSV.

- -o [OUTPUT FILE] – This argument is used to specify the output file to save the table data to. The default is to output to the console (i.e. your terminal window).

- [INPUT FILE] – This argument is used to specify the PDF file to extract tables from.

For example, if you wanted to extract a table from a PDF file named "example.pdf" and save the output as a CSV file named "output.csv", you would use the following command:

tabula -f csv -o output.csv example.pdf

Overall, Tabula is a powerful tool that can make it much easier to extract and analyze data from complex PDF files. With its flexible command-line options and support for multiple output formats, it is a great choice for anyone who needs to work with PDF data on a regular basis. 

## tldr 
 
> Extract tables from PDF files.
> More information: <https://tabula.technology>.

- Extract all tables from a PDF to a CSV file:

`tabula -o {{file.csv}} {{file.pdf}}`

- Extract all tables from a PDF to a JSON file:

`tabula --format JSON -o {{file.json}} {{file.pdf}}`

- Extract tables from pages 1, 2, 3, and 6 of a PDF:

`tabula --pages {{1-3,6}} {{file.pdf}}`

- Extract tables from page 1 of a PDF, guessing which portion of the page to examine:

`tabula --guess --pages {{1}} {{file.pdf}}`

- Extract all tables from a PDF, using ruling lines to determine cell boundaries:

`tabula --spreadsheet {{file.pdf}}`

- Extract all tables from a PDF, using blank space to determine cell boundaries:

`tabula --no-spreadsheet {{file.pdf}}`
