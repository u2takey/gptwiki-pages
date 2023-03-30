# mupdf 
## chatgpt 
mupdf is a command-line tool used to view and manipulate PDF documents. 

Here are some of the main features of mupdf:

1. View PDF documents: Mupdf allows you to view PDF documents in a clean and efficient interface. It has support for page zoom and rotation, bookmarks, search, and more.

2. Extract content: Mupdf can extract text and images from PDF documents. This can be useful if you need to copy text from a PDF, or if you want to export images for use in other applications.

3. Modify PDF documents: Mupdf can be used to modify existing PDF documents. You can insert, delete, or rearrange pages, add annotations, and modify text.

4. Convert PDF documents: Mupdf can convert PDF documents to other formats such as HTML, SVG, and text.

To use the mupdf command, simply open a terminal window and type "mupdf" followed by the path to the PDF document you want to view or manipulate. For example:

mupdf /path/to/my/document.pdf

This will open the document in the mupdf viewer. To access the various features of mupdf, you can use the keyboard shortcuts or the menus at the top of the window. 

## tldr 
 
> MuPDF is a lightweight PDF, XPS, and E-book viewer.
> More information: <https://www.mupdf.com>.

- Open a PDF on the first page:

`mupdf {{path/to/file}}`

- Open a PDF on page 3:

`mupdf {{path/to/file}} {{3}}`

- Open a password secured PDF:

`mupdf -p {{password}} {{path/to/file}}`

- Open a PDF with an initial zoom level, specified as DPI, of 72:

`mupdf -r {{72}} {{path/to/file}}`

- Open a PDF with inverted color:

`mupdf -I {{path/to/file}}`

- Open a PDF tinted red #FF0000 (hexadecimal color syntax RRGGBB):

`mupdf -C {{FF0000}}`

- Open a PDF without anti-aliasing (0 = off, 8 = best):

`mupdf -A {{0}}`
