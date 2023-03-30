# pdfjoin 
## chatgpt 
pdfjoin is a command-line tool that is used to join multiple PDF files into a single PDF file.

The basic syntax of the pdfjoin command is as follows:

pdfjoin [option] inputfile1 [<inputfile2> ...] [--output outputfile]

Here is what each part of this command does:

- pdfjoin: This is the command itself, which is used to join PDF files.
- [option]: This part of the command allows you to specify any optional parameters that you may want to use. For example, you can use the "--rotateoversize true" option to automatically rotate any pages that are oversized.
- inputfile1: This is the name of the first PDF file that you want to join. You can specify multiple input files if you want to join more than two PDF files into a single file.
- [<inputfile2> ...]: This part of the command allows you to specify additional input files, if you want to join more than two PDF files into a single file.
- [--output outputfile]: This part of the command is optional, and is used to specify the name of the output file. If you don't specify an output file, then pdfjoin will create a file with the same name as the first input file, with "_joined" added to the end.

Once you have all of your input files and options specified, you can run the pdfjoin command to join the PDF files together. Pdfjoin will create a new PDF file that contains all of the pages from each of the input files, in the order that they were specified on the command line. 

## tldr 
 
> PDF merging utility based on pdfjam.
> More information: <https://github.com/rrthomas/pdfjam-extras>.

- Merge two PDFs into one with the default suffix "joined":

`pdfjoin {{path/to/file1.pdf}} {{path/to/file2.pdf}}`

- Merge the first page of each given file together:

`pdfjoin {{path/to/file1.pdf path/to/file2.pdf ...}} {{1}} --outfile {{output_file}}`

- Save pages 3 to 5 followed by page 1 to a new PDF with custom suffix:

`pdfjoin {{path/to/file.pdf}} {{3-5,1}} --suffix {{rearranged}}`

- Merge page subranges from two PDFs:

`pdfjoin {/path/to/file1.pdf}} {{2-}} {{file2}} {{last-3}} --outfile {{output_file}}`
