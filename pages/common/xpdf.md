# xpdf 
## chatgpt 
xpdf is a command-line tool that is used to view and manipulate Portable Document Format (PDF) files on Unix-based systems. It is designed to be lightweight and efficient, making it a popular choice among users who want to quickly view and navigate PDF files without the need for a graphical user interface.

The xpdf command is typically used to open a PDF file in a terminal window or other command-line interface. To use xpdf, simply type "xpdf" followed by the name of the PDF file you want to view. For example:

```
xpdf my_file.pdf
```

This will open the PDF file "my_file.pdf" in a new window. Once the file is open, you can navigate through the document using the arrow keys or the scroll bar. You can also zoom in or out using the "+" and "-" keys, and you can search for specific text using the "/search_term" command.

In addition to viewing PDF files, xpdf also includes a number of other useful features, such as the ability to extract images or text from a PDF file, convert a PDF file to a PostScript file, or merge multiple PDF files into a single document. These features can be accessed using various command-line options, which can be found by typing "xpdf -h" or "man xpdf" in the terminal. 

## tldr 
 
> Portable Document Format (PDF) file viewer.
> More information: <https://www.xpdfreader.com/xpdf-man.html>.

- Open a PDF file:

`xpdf {{path/to/file.pdf}}`

- Open a specific page in a PDF file:

`xpdf {{path/to/file.pdf}} :{{page_number}}`

- Open a compressed PDF file:

`xpdf {{path/to/file.pdf.tar}}`

- Open a PDF file in fullscreen mode:

`xpdf -fullscreen {{path/to/file.pdf}}`

- Specify the initial zoom:

`xpdf -z {{75}}% {{path/to/file.pdf}}`

- Specify the initial zoom at page width or full page:

`xpdf -z {{page|width}} {{path/to/file.pdf}}`
