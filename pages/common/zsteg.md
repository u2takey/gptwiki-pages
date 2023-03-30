# zsteg 
## chatgpt 
zsteg is a command-line tool used for detecting steganography in PNG and BMP images. Steganography is the practice of hiding secret messages or data inside other image, audio, or video files, making it difficult for unauthorized users to detect or access.

When you run the zsteg command, it will analyze the image file and check for any hidden information, including text, binary data, or other file formats that may be embedded within the image.

To use the zsteg command, you need to install it first. You can install it on Linux, macOS, and Windows operating systems using different package managers.

To use it, open your terminal or command prompt and type “zsteg” followed by the name of the file you want to analyze. For example:

```zsteg my_image.png```

This command will run a scan for hidden data in the “my_image.png” file. If any hidden data is detected, it will display the results in the terminal, including the format of the data and its location within the image.

You can also use additional options with the zsteg command to specify different formats or data types to search for. Some of the common options include:

- ```-a``` to search for all formats
- ```-E``` to search for encrypted data
- ```-s <bits>``` to set the start bit
- ```-B``` to treat the file as a BMP image rather than a PNG image

Overall, zsteg is a useful tool for detecting steganography in image files and can help you identify potential security risks or hidden information that may be lurking in your image files. 

## tldr 
 
> Steganography detection tool for PNG and BMP file formats.
> It detects LSB steganography, ZLIB-compressed data, OpenStego, Camouflage and LSB with the Eratosthenes set.
> More information: <https://github.com/zed-0xff/zsteg>.

- Detect embedded data in a PNG:

`zsteg {{path/to/image.png}}`

- Detect embedded data in a BMP image, using all known methods:

`zsteg --all {{path/to/image.bmp}}`

- Detect embedded data in a PNG, iterating pixels vertically and using MSB first:

`zsteg --msb --order yx {{path/to/image.png}}`

- Detect embedded data in a BMP image, specifying the bits to consider:

`zsteg --bits {{1,2,3|1-3}} {{path/to/image.bmp}}`

- Detect embedded data in a PNG, extracting only prime pixels and inverting bits:

`zsteg --prime --invert {{path/to/image.png}}`

- Detect embedded data in a BMP image, specifying the minimum length of the strings to be found and the find mode:

`zsteg --min-str-len {{10}} --strings {{first|all|longest|none}} {{path/to/image.bmp}}`
