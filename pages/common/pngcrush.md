# pngcrush 
## chatgpt 
pngcrush is a command-line tool used to optimize and reduce the file size of PNG (Portable Network Graphics) images. It works by analyzing an input PNG image and finding ways to make it more efficient without sacrificing its quality.

The syntax of the pngcrush command follows the standard command line format: 

pngcrush inputfile.png outputfile.png

where 'inputfile' is the name of the PNG image to be optimized and 'outputfile' is the desired name for the optimized image.

Some of the features of pngcrush include: 

1. reducing the number of colors in an image
2. removing unnecessary metadata
3. compressing the image data with better filtering algorithms
4. converting the image to a more efficient color depth format, such as indexed or grayscale.

Overall, pngcrush is a useful tool for web designers and developers who want to reduce page load times and improve the performance of their websites by optimizing the PNG images they use. 

## tldr 
 
> PNG compression utility.
> More information: <https://pmt.sourceforge.io/pngcrush>.

- Compress a PNG file:

`pngcrush {{in.png}} {{out.png}}`

- Compress all PNGs and output them to the specified directory:

`pngcrush -d {{path/to/output}} *.png`

- Compress PNG file with all 114 available algorithms and pick the best result:

`pngcrush -rem allb -brute -reduce {{in.png}} {{out.png}}`
