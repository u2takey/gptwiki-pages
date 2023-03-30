# optipng 
## chatgpt 
OptiPNG is a command-line utility that is used for optimizing PNG (Portable Network Graphics) image files. This utility compresses the PNG images without any change on image quality, making the images take less space.

The OptiPNG command generally includes the following options and arguments:

1. -o: This option is used to set the optimization level for the image file. The range of values for this argument is 0-7, where 0 means no compression and 7 provides maximum compression.

2. -clobber: This option is used to overwrite the existing image with the optimized version.

3. -strip: This option is used to remove any unnecessary metadata from the image file, such as comments, author information, and creation date/time.

4. -preserve: This option is used when you want to preserve some of the metadata from the original file.

5. -quiet: This option is used to suppress all progress and error messages output by OptiPNG.

To execute OptiPNG, you should provide the path to the location of the image file(s) you want to optimize as arguments. For instance, the command to optimize an image in the current directory called image.png with maximum optimization level would be: 

optipng -o7 image.png 

## tldr 
 
> PNG file optimization utility.
> More information: <http://optipng.sourceforge.net>.

- Compress a PNG with default settings:

`optipng {{path/to/file.png}}`

- Compress a PNG with the best compression:

`optipng -o{{7}} {{path/to/file.png}}`

- Compress a PNG with the fastest compression:

`optipng -o{{0}} {{path/to/file.png}}`

- Compress a PNG and add interlacing:

`optipng -i {{1}} {{path/to/file.png}}`

- Compress a PNG and preserve all metadata (including file timestamps):

`optipng -preserve {{path/to/file.png}}`

- Compress a PNG and remove all metadata:

`optipng -strip all {{path/to/file.png}}`
