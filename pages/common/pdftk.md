# pdftk 
## chatgpt 
pdftk (PDF Toolkit) is a command-line tool used for manipulating PDF documents. It is used to perform various operations on PDF files, such as merging multiple PDF files into one, splitting a PDF into individual pages, encrypting and decrypting PDF files, adding watermarks and bookmarks, and many more.

The basic syntax of the pdftk command is:

pdftk input1.pdf input2.pdf … cat output output.pdf

This command takes one or more input PDF files, combines them using the "cat" command and creates a new output file called "output.pdf". Here's what each of the parts of this command does:

- "pdftk": This is the name of the command used to run the PDF Toolkit.
- "input1.pdf input2.pdf …": This is a list of one or more input PDF files that you want to manipulate. You can specify as many input files as you want by separating them with spaces.
- "cat": This is a command used to concatenate the input files. It is used when you want to merge multiple PDF files into a single document.
- "output": This specifies the name of the output PDF file that will be created. You can choose any name you want, but the file extension must be ".pdf".

Here are some other commonly used commands that can be used with pdftk:

- "split": Use this command to split a single PDF file into individual pages.
- "shuffle": Use this command to shuffle the pages of a PDF document.
- "burst": Use this command to split a PDF document into individual pages, but also create a separate file for each page.
- "uncompress": Use this command to uncompress a PDF document, which can help you access the document's raw data and metadata.

Overall, pdftk is a very powerful tool that can be used to manipulate PDF documents in many different ways. It is particularly useful for users who have to work with PDFs on a regular basis and need to automate certain tasks. 

## tldr 
 
> PDF toolkit.
> More information: <https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit>.

- Extract pages 1-3, 5 and 6-10 from a PDF file and save them as another one:

`pdftk {{input.pdf}} cat {{1-3 5 6-10}} output {{output.pdf}}`

- Merge (concatenate) a list of PDF files and save the result as another one:

`pdftk {{file1.pdf file2.pdf ...}} cat output {{output.pdf}}`

- Split each page of a PDF file into a separate file, with a given filename output pattern:

`pdftk {{input.pdf}} burst output {{out_%d.pdf}}`

- Rotate all pages by 180 degrees clockwise:

`pdftk {{input.pdf}} cat {{1-endsouth}} output {{output.pdf}}`

- Rotate third page by 90 degrees clockwise and leave others unchanged:

`pdftk {{input.pdf}} cat {{1-2 3east 4-end}} output {{output.pdf}}`
