# jpegtran 
## chatgpt 
jpegtran is a command-line utility program that is used to manipulate and transform JPEG files. It is a part of the Independent JPEG Group’s collection of utilities used for JPEG manipulations.

The jpegtran command has various options and flags that can be used to perform different operations on a JPEG file. Here are a few examples:

1. -copy none: This option is used to remove any metadata from the JPEG file such as EXIF data, comments, and markers.

2. -crop WxH+X+Y: This option is used to crop the JPEG image to the specified dimensions. WxH refers to the width and height of the cropped image, and X+Y refers to the coordinates of the cropped image.

3. -flip: This option is used to flip the JPEG image vertically.

4. -rotate X: This option is used to rotate the JPEG image by X degrees. The rotation can be clockwise or counterclockwise.

5. -scans file: This option is used to specify a file that contains a list of scans from the JPEG image. This can be used to extract certain parts of the JPEG image.

jpegtran can also be used in conjunction with other command-line utilities to perform more advanced operations on JPEG files. For example, you can use the Unix pipe command to pass the output of one command to the input of another command.

Overall, jpegtran is a powerful tool for manipulating and transforming JPEG files. Its options and flags make it a flexible tool for a variety of tasks. 

## tldr 
 
> Perform lossless transformation of JPEG files.
> More information: <https://manned.org/jpegtran>.

- Mirror an image horizontally or vertically:

`jpegtran -flip {{horizontal|vertical}} {{path/to/image.jpg}} > {{path/to/output.jpg}}`

- Rotate an image 90, 180 or 270 degrees clockwise:

`jpegtran -rotate {{90|180|270}} {{path/to/image.jpg}} > {{path/to/output.jpg}}`

- Transpose the image across the upper-left to lower right axis:

`jpegtran -transpose {{path/to/image.jpg}} > {{path/to/output.jpg}}`

- Transverse the image across the upper right to lower left axis:

`jpegtran -transverse {{path/to/image.jpg}} > {{path/to/output.jpg}}`

- Convert the image to grayscale:

`jpegtran -grayscale {{path/to/image.jpg}} > {{path/to/output.jpg}}`

- Crop the image to a rectangular region of width `W` and height `H` from the upper-left corner, saving the output to a specific file:

`jpegtran -crop {{W}}x{{H}} -outfile {{path/to/output.jpg}} {{path/to/image.jpg}}`

- Crop the image to a rectangular region of width `W` and height `H`, starting at point `X` and `Y` from the upper-left corner:

`jpegtran -crop {{W}}x{{H}}+{{X}}+{{Y}} {{path/to/image.jpg}} > {{path/to/output.jpg}}`
