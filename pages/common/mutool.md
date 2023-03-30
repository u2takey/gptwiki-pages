# mutool 
## chatgpt 
The command "mutool" is a command-line tool that is used for various PDF-related tasks. It is a part of MuPDF, which is a lightweight PDF and XPS viewer and toolkit.

The "mutool" command provides various command-line options to perform different operations on PDF files, such as merging, splitting, encrypting, decrypting, and optimizing. Here are some examples of different operations that can be performed using the "mutool" command:

- "mutool merge" is used to merge multiple PDF files into a single PDF file.
- "mutool split" is used to split a PDF file into multiple PDF files based on the number of pages or bookmarks.
- "mutool clean" is used to optimize PDF files by removing unused resources and compressing the file size.
- "mutool encrypt" is used to encrypt a PDF file with a password or certificate.
- "mutool decrypt" is used to decrypt a password-protected PDF file.
- "mutool extract" is used to extract text or images from a PDF file.

Overall, the "mutool" command allows users to manipulate PDF files using a command-line interface, which can be useful for automating tasks or integrating with other scripts or programs. 

## tldr 
 
> Convert PDF files, query information and extract data.
> More information: <https://mupdf.com/docs>.

- Convert pages 1-10 into 10 PNGs:

`mutool convert -o {{image%d.png}} {{file.pdf}} {{1-10}}`

- Convert pages 2, 3 and 5 of a PDF into text in the standard output:

`mutool draw -F {{txt}} {{file.pdf}} {{2,3,5}}`

- Concatenate two PDFs:

`mutool merge -o {{output.pdf}} {{input1.pdf}} {{input2.pdf}}`

- Query information about all content embedded in a PDF:

`mutool info {{input.pdf}}`

- Extract all images, fonts and resources embedded in a PDF out into the current directory:

`mutool extract {{input.pdf}}`

- Print the outline (table of contents) of a PDF:

`mutool show {{input.pdf}} outline`
