# pdfgrep 
## chatgpt 
pdfgrep is a command-line tool that can be used to search text in PDF documents. The tool is similar to the traditional grep command, but it is designed specifically to work with PDF files. 

The basic syntax of the pdfgrep command is as follows:

```
pdfgrep [OPTIONS] PATTERN [FILE...]
```

where OPTIONS represent command-line options or arguments, PATTERN represents the regular expression or text pattern to search, and the FILE represents the name of the PDF file(s) to search.

Some of the most common options available with the pdfgrep command include:

- -i, --ignore-case: searches for text patterns in a case-insensitive manner. 
- -r, --recursive: search files in subdirectories recursively.
- -n, --page-number: displays the page number of the matched text.
- -c, --count: displays the number of matches found.
- -o, --only-matching: displays only the matching text.

The pdfgrep command can be used for various purposes, such as searching for specific words or phrases in a PDF document, finding and replacing text, extracting text from PDF files, and more. The tool is efficient and flexible, making it a popular choice for text search and manipulation tasks. 

## tldr 
 
> Search text in PDF files.
> More information: <https://pdfgrep.org>.

- Find lines that match pattern in a PDF:

`pdfgrep {{pattern}} {{file.pdf}}`

- Include file name and page number for each matched line:

`pdfgrep --with-filename --page-number {{pattern}} {{file.pdf}}`

- Do a case-insensitive search for lines that begin with "foo" and return the first 3 matches:

`pdfgrep --max-count {{3}} --ignore-case {{'^foo'}} {{file.pdf}}`

- Find pattern in files with a `.pdf` extension in the current directory recursively:

`pdfgrep --recursive {{pattern}}`

- Find pattern on files that match a specific glob in the current directory recursively:

`pdfgrep --recursive --include {{'*book.pdf'}} {{pattern}}`
