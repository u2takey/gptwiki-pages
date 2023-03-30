# pdfinfo 
## chatgpt 
pdfinfo is a command-line tool that is used to display the detailed information about a PDF document. The command is used in the following syntax:

pdfinfo [options] filename.pdf

Options:
- -f n: Specifies the page number from which the information should be extracted.
- -l n: Specifies the page number till which information should be extracted.
- -meta: Display the meta information of the PDF file.
- -enc encoding: Specifies the encoding of the output.

Once the command is executed, it displays various information about the PDF file such as title, author, subject, keywords, page count, page size, PDF version, fonts used, etc. By default, pdfinfo displays information for all pages of the PDF document. However, if you want to extract information for a specific page or range of pages, you can use the -f and -l options along with the respective page numbers.

Overall, pdfinfo is a useful command that can help you extract valuable information about a PDF file quickly and easily. 

## tldr 
 
> Portable Document Format (PDF) file information viewer.
> More information: <https://www.xpdfreader.com/pdfinfo-man.html>.

- Print PDF file information:

`pdfinfo {{path/to/file.pdf}}`

- Specify user password for PDF file to bypass security restrictions:

`pdfinfo -upw {{password}} {{path/to/file.pdf}}`

- Specify owner password for PDF file to bypass security restrictions:

`pdfinfo -opw {{password}} {{path/to/file.pdf}}`
