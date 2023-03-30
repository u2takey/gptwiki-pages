# sam2p 
## chatgpt 
sam2p is a command-line tool used for converting raster image formats like GIF, PNG, BMP, and JPEG into the PDF format. It stands for Scalable Vector Graphics and Anti-Grain Geometry Postscript Processor.

The tool takes a command line argument followed by one or two filenames or Unix-style globs. It then converts the input file(s) into PDF format and saves it with the same name as the original file(s) but with a .pdf extension. Users can specify output resolution, page size and orientation, compression type and other conversion parameters using command-line options.

The sam2p tool uses a robust anti-aliasing engine to smooth out the pixels and generate high-quality vector graphics, which are scalable without losing quality. It is especially useful when creating PDF documents for web or print catalogs, posters, and other marketing materials.

Overall, sam2p is a powerful tool for converting raster image files into high-quality, scalable PDFs with a wide variety of customization options. It is available for use on Linux, macOS, and Windows operating systems. 

## tldr 
 
> Raster (bitmap) image converter with smart PDF and PostScript (EPS) output.
> More information: <http://pts.50.hu/sam2p/>.

- Concatenate all PDF files into one:

`sam2p *.pdf {{path/to/output.pdf}}`
