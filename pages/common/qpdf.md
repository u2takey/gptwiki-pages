# qpdf 
## chatgpt 
Qpdf is a command-line program that can be used to perform a variety of tasks related to PDF files. Here is a brief overview of the most common qpdf commands:

- `qpdf --encrypt=PASSWORD INPUT.pdf OUTPUT.pdf`: This command is used to encrypt a PDF file with a password. You must replace "PASSWORD" with the actual password you want to use. The input file is referred to as "INPUT.pdf" and the output file is referred to as "OUTPUT.pdf".
- `qpdf --decrypt INPUT.pdf OUTPUT.pdf`: This command is used to decrypt a password-protected PDF file. The input file is referred to as "INPUT.pdf" and the output file is referred to as "OUTPUT.pdf".
- `qpdf --rotate=[+/-]ANGLE:PAGE_RANGE INPUT.pdf OUTPUT.pdf`: This command is used to rotate one or more pages in a PDF file. You must replace "ANGLE" with the number of degrees you want to rotate the page(s). The optional "PAGE_RANGE" parameter is used to specify which pages you want to rotate. The input file is referred to as "INPUT.pdf" and the output file is referred to as "OUTPUT.pdf".
- `qpdf --split-pages=PAGE_RANGE INPUT.pdf OUTPUT.pdf`: This command is used to split a PDF file into multiple files, one for each page. The optional "PAGE_RANGE" parameter is used to specify which pages you want to split into separate files. The input file is referred to as "INPUT.pdf" and the output files will be named based on the page number.
- `qpdf --linearize INPUT.pdf OUTPUT.pdf`: This command is used to optimize a PDF file for web viewing. This can be useful if you have a large PDF file that takes too long to load in a web browser. The input file is referred to as "INPUT.pdf" and the output file is referred to as "OUTPUT.pdf".
- `qpdf --compress-streams=[gzip|zlib|none] INPUT.pdf OUTPUT.pdf`: This command is used to compress the streams in a PDF file to reduce the file size. You can specify "gzip", "zlib", or "none" as the compression type. The input file is referred to as "INPUT.pdf" and the output file is referred to as "OUTPUT.pdf".

These are just a few examples of the commands you can use with qpdf. You can find more options and details by reading the qpdf manual, which you can access by typing "man qpdf" in the terminal. 

## tldr 
 
> Versatile PDF transformation software.
> More information: <https://github.com/qpdf/qpdf>.

- Extract pages 1-3, 5 and 6-10 from a PDF file and save them as another one:

`qpdf --empty --pages {{input.pdf}} {{1-3,5,6-10}} -- {{output.pdf}}`

- Merge (concatenate) all the pages of a list of PDF files and save the result as a new PDF:

`qpdf --empty --pages {{file1.pdf}} {{file2.pdf}} {{file3.pdf}} -- {{output.pdf}}`

- Merge (concatenate) given pages from a list of PDF files and save the result as a new PDF:

`qpdf --empty --pages {{file1.pdf}} {{1,6-8}} {{file2.pdf}} {{3,4,5}} -- {{output.pdf}}`

- Write each group of n pages to a separate output file with a given filename pattern:

`qpdf --split-pages=n {{input.pdf}} {{out_%d.pdf}}`

- Rotate certain pages of a PDF with a given angle:

`qpdf --rotate={{90:2,4,6}} --rotate={{180:7-8}} {{input.pdf}} {{output.pdf}}`

- Remove the password from a password-protected file:

`qpdf --password={{password}} --decrypt {{input.pdf}} {{output.pdf}}`
