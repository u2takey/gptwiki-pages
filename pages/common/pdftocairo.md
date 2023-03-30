# pdftocairo 
## chatgpt 
pdftocairo is a command-line tool that is used to convert PDF files to image files using the Cairo 2D graphics library. The tool is available for multiple operating systems, including Linux, macOS, and Windows.

When using the pdftocairo command, you need to specify the input PDF file, the output image format, and the output file name. You can also set options to control the resolution, page range, and image compression.

Here is the basic usage of the pdftocairo command:

```
pdftocairo [options] <input.pdf> <output.<format>>
```

Here are some of the most commonly used options:

- `-r <resolution>`: Specifies the output resolution in dots per inch (dpi). The default is 150 dpi.
- `-f <first-page>`: Specifies the first page to convert. The default is 1.
- `-l <last-page>`: Specifies the last page to convert. The default is the last page in the file.
- `-jpeg`, `-png`, `-tiff`, or `-svg`: Specifies the output image format. The default is PNG.

For example, to convert the first page of a PDF file to a PNG image with a resolution of 300 dpi, you can use the following command:

```
pdftocairo -f 1 -l 1 -r 300 input.pdf output.png
```

This will create a PNG image file named "output.png" in the same directory as the input PDF file. 

## tldr 
 
> Converts PDF files to PNG/JPEG/TIFF/PDF/PS/EPS/SVG using cairo.
> More information: <https://poppler.freedesktop.org>.

- Convert a PDF file to JPEG:

`pdftocairo {{path/to/file.pdf}} -jpeg`

- Convert to PDF expanding the output to fill the paper:

`pdftocairo {{path/to/file.pdf}} {{output.pdf}} -pdf -expand`

- Convert to SVG specifying the first/last page to convert:

`pdftocairo {{path/to/file.pdf}} {{output.svg}} -svg -f {{first_page}} -l {{last_page}}`

- Convert to PNG with 200ppi resolution:

`pdftocairo {{path/to/file.pdf}} {{output.png}} -png -r 200`

- Convert to grayscale TIFF setting paper size to A3:

`pdftocairo {{path/to/file.pdf}} -tiff -gray -paper A3`

- Convert to PNG cropping x and y pixels from the top-left corner:

`pdftocairo {{path/to/file.pdf}} -png -x {{x_pixels}} -y {{y_pixels}}`
