# diff-pdf 
## chatgpt 
diff-pdf is a command-line program used to compare and highlight differences between two PDF files. Here is more detail on the command:

- Syntax: diff-pdf [options] FILE1 FILE2 [, output]

- Options: diff-pdf has several command-line options that you can use to customize the output or behavior, including specifying a page range to compare, adjusting the level of detail in the output, specifying an output format, and more.

- FILE1 and FILE2: These are the two PDF files you want to compare.

- Output: diff-pdf will display its output in the command line by default. However, you can also specify an output format (like HTML or XML) and direct the output to a file if you like.

- How it works: diff-pdf works by analyzing the structure and content of each PDF and comparing them to each other. Any differences in the two files are highlighted in the output, such as changes in text, images, or page layout. The output can also include a summary of the number and type of changes detected.

- Use cases: diff-pdf is useful for a variety of scenarios, such as comparing two versions of the same document or verifying that a PDF file was not altered in transit. It can also help identify any formatting or content issues that may have occurred during conversion from another file format (like Word or Excel) to PDF.

Overall, diff-pdf is a powerful command-line tool for analyzing and comparing PDF files. Its flexible options and detailed output make it a valuable addition to any file management or quality control process. 

## tldr 
 
> Tool for comparing two PDFs.
> More information: <https://github.com/vslavik/diff-pdf>.

- Compare PDFs, indicating changes using return codes (`0` = no difference, `1` = PDFs differ):

`diff-pdf {{path/to/a.pdf}} {{path/to/b.pdf}}`

- Compare PDFs, outputting a PDF with visually highlighted differences:

`diff-pdf --output-diff={{path/to/diff.pdf}} {{path/to/a.pdf}} {{path/to/b.pdf}}`

- Compare PDFs, viewing differences in a simple GUI:

`diff-pdf --view {{path/to/a.pdf}} {{path/to/b.pdf}}`
