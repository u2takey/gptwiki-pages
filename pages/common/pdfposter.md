# pdfposter 
## chatgpt 
pdfposter is a command-line tool used for creating large-format PDF documents by splitting and scaling the original PDF pages into multiple smaller pages that can be printed and assembled into a poster. The command works by taking an input PDF file and converting it into a poster format by specifying the number of pages that the original PDF page should be split into.

The syntax of the pdfposter command is as follows:

pdfposter [options] input_file output_file

Options:
-d, --dim=WIDTHxHEIGHT: specifies the size of the output poster in millimeters or inches
-a, --paper=A4/A3/…: sets the output to a standard paper size
-p, --poster=COLxROW: specifies the number of columns and rows of the poster
-m, --margins=LEFTxRIGHTxTOPxBOTTOM: sets the margins of the poster in millimeters or inches
-s, --scale=SCALE: scales the input page by the specified factor
-r, --overlap=OVERLAP: specifies the overlap between the pages of the poster
-f, --fit=NONE/TIGHT/SHRINK/STRETCH: adjusts the output page to fit the poster dimensions
-v, --verbose: displays detailed information about the conversion process

Input_file: The PDF file that needs to be converted into a poster format.

Output_file: The name of the output file.

In summary, the pdfposter command is used to create large-format PDF documents by splitting and scaling the original PDF pages into multiple smaller pages that can be printed and assembled into a poster. 

## tldr 
 
> Convert a large-sheeted PDF into multiple A4 pages for printing.
> More information: <https://pdfposter.readthedocs.io>.

- Convert an A2 poster into 4 A4 pages:

`pdfposter --poster-size a2 {{input_file.pdf}} {{output_file.pdf}}`

- Scale an A4 poster to A3 and then generate 2 A4 pages:

`pdfposter --scale 2 {{input_file.pdf}} {{output_file.pdf}}`
