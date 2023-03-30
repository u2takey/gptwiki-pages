# pdffonts 
## chatgpt 
`pdffonts` is a command-line tool that allows users to analyze the fonts used in a PDF file. When executed, `pdffonts` parses a PDF file and outputs a report containing all the font types used, the number of pages that use each font, the font's name, and the size of each font in the document.

For each font used in the document, `pdffonts` provides information such as the type of font (TrueType, Type 1, etc.), the encoding method used (Standard, Unicode, etc.), and if the font is embedded or not.

The `pdffonts` tool can be useful for diagnosing font-related issues in a PDF document. It can be used to determine if a particular font is not embedded in the PDF file and may cause issues when displayed on a different computer. It can also be used to identify fonts that are unused or very large, which may affect the overall file size.

To use `pdffonts`, simply open the command prompt or terminal on your computer, navigate to the location of the PDF file and enter the command `pdffonts filename.pdf`. The tool will then generate a report of all the fonts used in the document. 

## tldr 
 
> Portable Document Format (PDF) file fonts information viewer.
> More information: <https://www.xpdfreader.com/pdffonts-man.html>.

- Print PDF file fonts information:

`pdffonts {{path/to/file.pdf}}`

- Specify user password for PDF file to bypass security restrictions:

`pdffonts -upw {{password}} {{path/to/file.pdf}}`

- Specify owner password for PDF file to bypass security restrictions:

`pdffonts -opw {{password}} {{path/to/file.pdf}}`

- Print additional information on location of the font that will be used when the PDF file is rasterized:

`pdffonts -loc {{path/to/file.pdf}}`

- Print additional information on location of the font that will be used when the PDF file is converted to PostScript:

`pdffonts -locPS {{path/to/file.pdf}}`
