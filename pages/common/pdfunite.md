# pdfunite 
## chatgpt 
pdfunite is a command-line utility used to merge multiple PDF files into a single PDF. The command works on Linux, macOS, and other Unix-like systems. 

The syntax for the pdfunite command is as follows:

```
pdfunite [OPTIONS] INFILES... OUTFILE
```

where:
- [OPTIONS]: any command-line options that you want to use with the pdfunite command
- INFILES: the input PDF files that you want to merge. You can specify multiple files by separating them with a space.
- OUTFILE: the name for the output PDF file that will contain the merged content from the input files.

Here are some of the most commonly used options for the pdfunite command:

- -f, --first-page: specifies the first page to include from the input files
- -l, --last-page: specifies the last page to include from the input files
- -o, --output: specifies the output file's name and location

Example usage:

```
pdfunite file1.pdf file2.pdf file3.pdf merged.pdf
```

This command will merge the contents of file1.pdf, file2.pdf, and file3.pdf into a new file called merged.pdf.

```
pdfunite -o /path/to/merged.pdf file1.pdf file2.pdf
```

This command will merge the contents of file1.pdf and file2.pdf into a new file called merged.pdf, which will be saved in the directory specified by the /path/to/ path. 

## tldr 
 
> PDF merging utility.
> More information: <https://github.com/mtgrosser/pdfunite>.

- Merge 2 PDFs into a single PDF:

`pdfunite {{path/to/fileA.pdf}} {{path/to/fileB.pdf}} {{path/to/merged_output.pdf}}`

- Merge a directory of PDFs into a single PDF:

`pdfunite {{path/to/directory/*.pdf}} {{path/to/merged_output.pdf}}`
