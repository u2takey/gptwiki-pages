# gs 
## chatgpt 
"gs" is the shorthand command for the Ghostscript application, which is a freely available interpreter for the PostScript language and for PDF (Adobe Acrobat) files. Ghostscript allows for the processing and manipulation of PostScript or PDF files using various parameters and options.

When invoking the "gs" command, the user typically includes various parameters and options after the initial command, such as the input file name, output file name, resolution, and page range. For example, one might use the following command to convert a PostScript file to a PDF file:

gs -sDEVICE=pdfwrite -sOutputFile=example.pdf example.ps 

In this command, the "-sDEVICE" option specifies the output device as pdfwrite, while the "-sOutputFile" option specifies the name of the output file as "example.pdf". The input file name is also provided after the options, in this case "example.ps".

The Ghostscript application includes a wide range of parameters and options that users can use to control how the file is processed and outputted. These parameters allow for things such as resolution adjustment, image compression, font embedding, and many other features. By using the "gs" command with these options, users can manipulate and process PostScript and PDF files with precision and flexibility. 

## tldr 
 
> GhostScript is a PDF and PostScript interpreter.
> More information: <https://manned.org/gs>.

- To view a file:

`gs -dQUIET -dBATCH {{file.pdf}}`

- Reduce PDF file size to 150 dpi images for reading on a e-book device:

`gs -dNOPAUSE -dQUIET -dBATCH -sDEVICE=pdfwrite -dPDFSETTINGS=/ebook -sOutputFile={{output.pdf}} {{input.pdf}}`

- Convert PDF file (pages 1 through 3) to an image with 150 dpi resolution:

`gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=jpeg -r150 -dFirstPage={{1}} -dLastPage={{3}} -sOutputFile={{output_%d.jpg}} {{input.pdf}}`

- Extract pages from a PDF file:

`gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input.pdf}}`

- Merge PDF files:

`gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input1.pdf}} {{input2.pdf}}`

- Convert from PostScript file to PDF file:

`gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input.ps}}`
