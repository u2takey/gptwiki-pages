# cwebp 
## chatgpt 
cwebp is a command-line tool used for encoding images in the WebP format. WebP is an image format developed by Google that provides lossless and lossy compression for images on the web.

The cwebp command takes an input file, usually in PNG, JPEG, or BMP format, and converts it into a WebP format file. It offers a variety of options that can be used to specify the encoding parameters, such as quality level, alpha compression, and down-sampling.

Some of the commonly used options with the cwebp command include:

- -q: Sets the quality level of the output image. The value can range from 0 to 100, where 100 is the highest quality and 0 is the lowest.
- -alpha_q: Sets the quality level of the alpha channel (if present) in the output image.
- -lossless: Encodes the image in a lossless format, avoiding any compression loss but typically resulting in larger file sizes.
- -resize: Resizes the image to the specified dimensions. This can be useful for optimizing image sizes for web usage.
- -hazy: Applies a haze effect to the output image.

The cwebp command is available for Windows, macOS, and Linux platforms and can be used in batch processing workflows for large numbers of images. It is a powerful tool for optimizing image sizes while maintaining high-quality visuals on the web. 

## tldr 
 
> Compress an image file to a WebP file.
> More information: <https://developers.google.com/speed/webp/docs/cwebp>.

- Compress a WebP file with default settings (q = 75) to the [o]utput file:

`cwebp {{path/to/image_file}} -o {{path/to/output.webp}}`

- Compress a WebP file with the best [q]uality and largest file size:

`cwebp {{path/to/image_file}} -o {{path/to/output.webp}} -q {{100}}`

- Compress a WebP file with the worst [q]uality and smallest file size:

`cwebp {{path/to/image_file}} -o {{path/to/output.webp}} -q {{0}}`

- Compress a WebP file and apply resize to image:

`cwebp {{path/to/image_file}} -o {{path/to/output.webp}} -resize {{width}} {{height}}`

- Compress a WebP file and drop alpha channel information:

`cwebp {{path/to/image_file}} -o {{path/to/output.webp}} -noalpha`
