# inkview 
## chatgpt 
Inkview is a command-line tool used to view and convert ink annotations in PDF documents. It is part of the Xournal suite of tools for working with handwritten notes, sketches, and annotations.

The basic usage of inkview is:

    inkview [options] <input-file>

The options available with inkview include:

- `-o, --output`: specify the output file name or format. By default, inkview outputs to PNG format. Other formats that can be specified include SVG, PDF, and Xournal.
- `-p, --page`: specify the page number to view or convert.
- `-l, --layer`: specify the layer to view or convert. This is useful for PDF documents that have multiple layers of ink annotations.
- `-s, --size`: specify the output image size. This can be a percentage of the original size or a specific width or height in pixels.
- `-r, --resolution`: specify the output image resolution in dots per inch.
- `-n, --no-preview`: run inkview in batch mode with no preview window.

When you run the inkview command, it will display the specified page and ink annotations in a graphical window. You can interact with the annotations using your mouse or touchpad. Inkview also provides a toolbar with various tools for selecting, erasing, and modifying ink annotations.

If you want to convert the annotations to a different format or save them to a file, you can use one of the output options with inkview. For example, to convert a PDF page with ink annotations to SVG format, you can run:

    inkview -o output.svg -p 2 input.pdf

This will create a new SVG file called "output.svg" that contains the ink annotations from page 2 of the input PDF file. 

## tldr 
 
> Inkscape graphical SVG previewer.
> Also functions as a slideshow viewer.
> More information: <http://wiki.inkscape.org/wiki/index.php/Inkview>.

- Preview an SVG:

`inkview {{path/to/file.svg}}`

- Preview multiple SVGs (use arrow keys to navigate):

`inkview {{path/to/file_a.svg}} {{path/to/file_b.svg}} {{path/to/file_c.svg}}`
