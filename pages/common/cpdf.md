# cpdf 
## chatgpt 
cpdf is a command line tool for manipulating PDF documents. It provides a range of functions for editing and modifying PDF files, including adding or removing pages, merging or spliting documents, changing page orientation, adding watermarks, and more. 

The general syntax for using cpdf command is:

```
cpdf operation [arguments] input.pdf -o output.pdf
```

- "operation" specifies the specific action to be performed on the PDF file.
- "arguments" are optional parameters that may be needed for the operation.
- "input.pdf" is the path to the input PDF file.
- "-o" is a flag indicating that the output file should be saved to a new file.
- "output.pdf" is the path to the output PDF file.

Here are some examples of using cpdf:

1. Merge multiple PDF files into one:

```
cpdf one.pdf two.pdf three.pdf -o combined.pdf
```

This command will merge the three input PDF files (one.pdf, two.pdf, and three.pdf) into a single output file named combined.pdf.

2. Add a watermark to every page of a PDF file:

```
cpdf input.pdf -stamp-under "watermark.pdf" -o output.pdf
```

This command will add a watermark (provided in the file "watermark.pdf") under every page of the input file (input.pdf), and save the output to a new file (output.pdf).

3. Rotate every page in a PDF file:

```
cpdf input.pdf -rotate "90" -o output.pdf
```

This command will rotate every page of the input file by 90 degrees, and save the output to a new file named output.pdf. 

Overall, cpdf is a powerful command line tool for performing various operations on PDF files quickly and efficiently. 

## tldr 
 
> CLI to manipulate existing PDF files in a variety of ways.
> More information: <https://www.coherentpdf.com/cpdfmanual/cpdfmanual.html>.

- Select pages 1, 2, 3 and 6 from a source document and write those to a destination document:

`cpdf {{path/to/source_document.pdf}} {{1-3,6}} -o {{path/to/destination_document.pdf}}`

- Merge two documents into a new one:

`cpdf -merge {{path/to/source_document_one.pdf}} {{path/to/source_document_two.pdf}} -o {{path/to/destination_document.pdf}}`

- Show the bookmarks of a document:

`cpdf -list-bookmarks {{path/to/document.pdf}}`

- Split a document into ten-page chunks, writing them to `chunk001.pdf`, `chunk002.pdf`, etc:

`cpdf -split {{path/to/document.pdf}} -o {{path/to/chunk%%%.pdf}} -chunk {{10}}`

- Encrypt a document using 128bit encryption, providing `fred` as owner password and `joe` as user password:

`cpdf -encrypt {{128bit}} {{fred}} {{joe}} {{path/to/source_document.pdf}} -o {{path/to/encrypted_document.pdf}}`

- Decrypt a document using the owner password `fred`:

`cpdf -decrypt {{path/to/encrypted_document.pdf}} owner={{fred}} -o {{path/to/decrypted_document.pdf}}`

- Show the annotations of a document:

`cpdf -list-annotations {{path/to/document.pdf}}`

- Create a new document from an existing one with additional metadata:

`cpdf -set-metadata {{path/to/metadata.xml}} {{path/to/source_document.pdf}} -o {{path/to/destination_document.pdf}}`
