# pdfseparate 
## chatgpt 
pdfseparate is a command-line tool (also known as a terminal command) for splitting a single PDF document into multiple PDF files. It is part of the Poppler PDF utilities package, which is available for Linux, Unix, and Windows operating systems.

To use pdfseparate, you need to open a terminal window and type the command, along with the required arguments and options.

The basic syntax of pdfseparate command is:

pdfseparate input_file.pdf output_file_prefix%03d.pdf [page_range]

Here, input_file.pdf is the name of the PDF file you want to split, output_file_prefix is the name prefix for the output files (with %03d representing the page number), and page_range specifies the range of pages you want to split (in the format of start_page-end_page).

For example, if you type the following command:

pdfseparate mydoc.pdf myfiles%03d.pdf 1-5

It will split the PDF file "mydoc.pdf" into five separate files, with the name prefix "myfiles" and page numbers from 001 to 005 (i.e., myfiles001.pdf, myfiles002.pdf, etc.), containing pages 1 to 5 of the original file.

You can also use various options with the pdfseparate command to customize the output files, such as specifying a different file format (e.g., JPEG or PNG) or DPI (dots per inch) for the images of each page.

Overall, pdfseparate is a useful tool for splitting large PDF files into smaller ones for easier management and distribution. 

## tldr 
 
> Portable Document Format (PDF) file page extractor.
> More information: <https://manpages.debian.org/unstable/poppler-utils/pdfseparate.1.en.html>.

- Extract pages from PDF file and make a separate PDF file for each page:

`pdfseparate {{path/to/source_filename.pdf}} {{path/to/destination_filename-%d.pdf}}`

- Specify the first/start page for extraction:

`pdfseparate -f {{3}} {{path/to/source_filename.pdf}} {{path/to/destination_filename-%d.pdf}}`

- Specify the last page for extraction:

`pdfseparate -l {{10}} {{path/to/source_filename.pdf}} {{path/to/destination_filename-%d.pdf}}`
