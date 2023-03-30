# pdfxup 
## chatgpt 
As an AI language model, I am not aware of the specific command "pdfxup." It is possible that this command has been created for a specific software or program that I do not have knowledge on. Could you please provide more context on where this command is being used and what software or program it belongs to? This will help me provide you with a more accurate explanation. 

## tldr 
 
> N-up PDF pages.
> N-upping means putting multiple pages onto one page by scaling and rotating them into a grid.
> More information: <https://ctan.org/pkg/pdfxup>.

- Create a 2-up PDF:

`pdfxup -o {{path/to/output.pdf}} {{path/to/input.pdf}}`

- Create a PDF with 3 columns and 2 lines per page:

`pdfxup -x {{3}} -y {{2}} -o {{path/to/output.pdf}} {{path/to/input.pdf}}`

- Create a PDF in booklet mode (2-up, and pages are sorted to form a book when folded):

`pdfxup -b -o {{path/to/output.pdf}} {{path/to/input.pdf}}`
