# img2pdf 
## chatgpt 
Img2pdf is a command-line tool that allows the user to convert one or more image files to a PDF document. The command "img2pdf" is used to call the img2pdf tool.

Here is a breakdown of the different elements of the command:

- img2pdf: The command itself that is used to call the img2pdf tool.

- [OPTIONS]: This part of the command is optional and allows the user to specify additional options for the conversion. These options can include things like the output file name, compression level, image resolution, and more. Some commonly used options are:

  - -o or --output: Specifies the name of the output PDF file. This option is followed by the desired name of the output file.
  
  - -r or --resolution: Sets the resolution of the output PDF in DPI. This option is followed by a number representing the desired DPI.
  
  - -C or --compression: Specifies the level of compression applied to the output PDF file. Options range from 0 (no compression) to 3 (maximum compression).

- file1.jpg [file2.jpg … fileN.jpg]: This part of the command specifies the input image files that need to be converted to a PDF. The command allows for multiple image files to be converted in one go, with each file separated by a space.

Overall, the img2pdf command is a simple yet powerful command-line tool that can quickly convert image files to a PDF document with various customization options. 

## tldr 
 
> Command-line lossless converter of raster images to PDF.
> More information: <https://gitlab.mister-muffin.de/josch/img2pdf>.

- Convert multiple images to a single PDF, each image being on its own page:

`img2pdf {{path/to/image1.jpg}} {{path/to/image2.jpg}} --output {{path/to/file.pdf}}`

- Convert only the first frame of a multi-frame image to PDF:

`img2pdf {{path/to/file.gif}} --first-frame-only --output {{path/to/file.pdf}}`

- Auto orient the image, use a page size of A4 in landscape mode, and set a border of 2cm horizontally and 5.1cm vertically:

`img2pdf {{path/to/file.jpg}} --auto-orient --pagesize {{A4^T}} --border {{2cm}}:{{5.1cm}} --output {{path/to/file.pdf}}`

- Shrink only larger images to a 10cm by 15cm rectangle inside a 30x20cm page:

`img2pdf {{path/to/file.tiff}} --pagesize {{30cm}}x{{20cm}} --imgsize {{10cm}}x{{15cm}} --fit {{shrink}} --output {{path/to/file.pdf}}`

- Convert an image to PDF, and specify metadata for the resulting file:

`img2pdf {{path/to/file.png}} --title {{title}} --author {{author}} --creationdate {{1970-01-31}} --keywords {{keyword1 keyword2}} --subject {{subject}} --output {{path/to/file.pdf}}`
