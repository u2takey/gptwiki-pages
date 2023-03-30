# pdftoppm 
## chatgpt 
The pdftoppm command is a command line tool that is used to convert PDF documents to Portable Pixmap (PPM) image format. This command is installed as part of the poppler-utils package on most Linux systems.

Syntax:

pdftoppm [options] [PDF-file] [PPM-file-prefix]

The command can take the following options:

- -f <int> : Specifies the first page to convert from the PDF file
- -l <int> : Specifies the last page to convert from the PDF file
- -r <int> : Specifies the resolution in DPI (dots per inch)
- -gray : Converts the PDF to grayscale
- -mono : Converts the PDF to black and white
- -jpeg : Converts the PDF to a JPEG image
- -png : Converts the PDF to a PNG image
- -tiff : Converts the PDF to a TIFF image
- -cropbox : Uses the crop box instead of the media box for page rendering
- -q : Sets the rendering quality (0-100, with 100 being the highest quality)
- -h : Displays help information about the command

The [PDF-file] parameter specifies the path and name of the PDF file that is to be converted. The [PPM-file-prefix] parameter specifies the prefix that will be used when naming the PPM image files. The output image files will be named with a sequential number followed by the prefix.

For example, the command to convert a PDF to PPM format with a resolution of 300 DPI would be:

pdftoppm -r 300 input.pdf output-prefix 

## tldr 
 
> Convert PDF document pages to portable Pixmap (image formats).
> More information: <https://manned.org/pdftoppm>.

- Specify the range of pages to convert (N-first page, M-last page):

`pdftoppm -f {{N}} -l {{M}} {{path/to/file.pdf}} {{image_name_prefix}}`

- Convert only the first page of a PDF:

`pdftoppm -singlefile {{path/to/file.pdf}} {{image_name_prefix}}`

- Generate a monochrome PBM file (instead of a color PPM file):

`pdftoppm -mono {{path/to/file.pdf}} {{image_name_prefix}}`

- Generate a grayscale PGM file (instead of a color PPM file):

`pdftoppm -gray {{path/to/file.pdf}} {{image_name_prefix}}`

- Generate a PNG file instead a PPM file:

`pdftoppm -png {{path/to/file.pdf}} {{image_name_prefix}}`
