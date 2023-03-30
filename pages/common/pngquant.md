# pngquant 
## chatgpt 
pngquant is a command-line tool used to optimize PNG images without compromising the quality. It uses a lossy compression algorithm that reduces the number of colors in the image while preserving the overall quality of the image, making it smaller in size and easier to load on web pages. 

Here's how the command works: 

1. pngquant requires a PNG file as input. So, the first step is to specify the path to the PNG file that needs to be optimized. 

2. pngquant also allows users to specify a number of options to control the compression process. These options include the number of colors to reduce the image to, the quality of the output file, and the dithering method used. 

3. Once the options are specified, the pngquant command is executed, and the optimization process begins. pngquant reduces the number of colors in the image while preserving the image's overall appearance to produce a smaller, optimized PNG file. 

4. The optimized PNG file is then saved to the specified location, overwriting the original file if desired. 

Overall, the pngquant command is a useful tool for web developers and designers looking to optimize their websites and reduce page load times. By compressing PNG files, users can achieve faster load times, better user experience, and improved SEO. 

## tldr 
 
> PNG converter and lossy image compressor.
> More information: <https://pngquant.org/>.

- Compress a specific PNG as much as possible and write result to a new file:

`pngquant {{path/to/file.png}}`

- Compress a specific PNG and override original:

`pngquant --ext .png --force {{path/to/file.png}}`

- Try to compress a specific PNG with custom quality (skip if below the min value):

`pngquant --quality {{0-100}} {{path/to/file.png}}`

- Compress a specific PNG with the number of colors reduced to 64:

`pngquant {{64}} {{path/to/file.png}}`

- Compress a specific PNG and skip if the file is larger than the original:

`pngquant --skip-if-larger {{path/to/file.png}}`

- Compress a specific PNG and remove metadata:

`pngquant --strip {{path/to/file.png}}`

- Compress a specific PNG and save it to the given path:

`pngquant {{path/to/file.png}} --output {{path/to/file.png}}`

- Compress a specific PNG and show progress:

`pngquant --verbose {{path/to/file.png}}`
