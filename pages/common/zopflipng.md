# zopflipng 
## chatgpt 
ZopfliPNG is a command-line tool that is used to compress PNG images losslessly. It is an open-source compression algorithm that is designed to optimize the size of the PNG files without sacrificing the quality of the image. Here are some of the key features of the zopflipng command:

1. Lossless compression: ZopfliPNG uses a lossless compression algorithm that reduces the size of the PNG files without losing any data or image quality.

2. Faster compression: ZopfliPNG is designed to be faster than other compression tools such as PNGOUT and OptiPNG. It achieves this by implementing multi-threading and other optimization techniques.

3. Small file sizes: ZopfliPNG produces smaller file sizes compared to other compression tools, without compromising image quality.

4. Command-line interface: ZopfliPNG is a command-line tool that is easy to use, and it can be integrated into automated workflows.

To use the zopflipng command, you need to open a terminal or command prompt, navigate to the directory where the PNG files are located, and then run the command followed by the filename of the PNG file you want to compress. Here's an example command:

zopflipng -m 8 -y file.png output.png

In this command, "-m 8" is an option that controls the compression level. Higher values of "m" result in better compression but take longer to process the image. "-y" is an option that tells zopflipng to overwrite the output file if it already exists. "file.png" is the name of the input file, and "output.png" is the name of the compressed file that will be created. Once the command completes, the compressed file will be located in the same directory as the input file, and its size will be reduced without compromising the quality of the image. 

## tldr 
 
> PNG compression utility.
> More information: <https://github.com/google/zopfli>.

- Optimize a PNG:

`zopflipng {{input.png}} {{output.png}}`

- Optimize several PNGs and save with given prefix:

`zopflipng --prefix={{prefix}} {{image1.png}} {{image2.png}} {{image3.png}}`
