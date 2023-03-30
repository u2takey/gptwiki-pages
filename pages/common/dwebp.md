# dwebp 
## chatgpt 
dwebp is a command-line tool that is used to decode and convert WebP images to other formats such as PNG or JPEG. Here is a detailed explanation of the command and its options:

Syntax: dwebp [options] input_file.webp [-o output_file]

Options:
-quiet: This option suppresses the output of the decoder.
-noasm: This option disables the use of assembly code.
-alpha_dither: This option adds dithering to alpha transparency.
-hint: This option enables hints from the WebP file.
-map: This option maps the alpha channel to either 1, 2, or 4 bits.
-yuv: This option enables YUV color space decoding.
-v: This option shows the version of dwebp.
-o: This option specifies the output file.

Example:
To convert a WebP image named "image.webp" to a PNG file named "image.png", use the following command:

dwebp image.webp -o image.png

This will convert the WebP image to a PNG file and save it with the specified name. 

## tldr 
 
> `dwebp` decompresses WebP files into PNG, PAM, PPM or PGM images.
> Animated WebP files are not supported.
> More information: <https://developers.google.com/speed/webp/docs/dwebp/>.

- Convert a `webp` file into a `png` file:

`dwebp {{path/to/input.webp}} -o {{path/to/output.png}}`

- Convert a `webp` file into a specific filetype:

`dwebp {{path/to/input.webp}} -bmp|-tiff|-pam|-ppm|-pgm|-yuv -o {{path/to/output}}`

- Convert a `webp` file, using multi-threading if possible:

`dwebp {{path/to/input.webp}} -o {{path/to/output.png}} -mt`

- Convert a `webp` file, but also crop and scale at the same time:

`dwebp {{input.webp}} -o {{output.png}} -crop {{x_pos}} {{y_pos}} {{width}} {{height}} -scale {{width}} {{height}}`

- Convert a `webp` file and flip the output:

`dwebp {{path/to/input.webp}} -o {{path/to/output.png}} -flip`

- Convert a `webp` file and don't use in-loop filtering to speed up the decoding process:

`dwebp {{path/to/input.webp}} -o {{path/to/output.png}} -nofilter`
