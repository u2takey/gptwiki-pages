# pdf-parser 
## chatgpt 
pdf-parser is a command-line tool that can be used to analyze and manipulate PDF files. It can parse and output the structure of a PDF file in a human-readable format, allowing users to inspect the contents of the file, including objects, streams, and metadata. 

The pdf-parser command typically takes a PDF file as input, and allows users to perform various operations on it, such as extracting specific objects or streams, searching for specific keywords, or decompressing streams.

Some examples of commonly used pdf-parser flags and options include:

- `-s`: Search for a keyword in the PDF file. This option can be used to locate specific content within the file, such as a particular image or font.
- `-r`: Recursively analyze all embedded objects within the PDF file. This can be useful for discovering hidden content or malware that may be embedded within the file.
- `-d`: Decompress all compressed streams within the PDF file, making it easier to read and analyze the contents.
- `-o`: Output a specific object within the PDF file to a separate file. This can be useful for extracting embedded images or other objects.

Overall, pdf-parser is a powerful tool for analyzing and manipulating PDF files, and can be particularly useful for security researchers or others who need to inspect the contents of PDF files in-depth. 

## tldr 
 
> Identify fundamental elements of a PDF file without rendering it.
> More information: <https://blog.didierstevens.com/programs/pdf-tools>.

- Display statistics for a PDF file:

`pdf-parser --stats {{path/to/file.pdf}}`

- Display objects of type `/Font` in a PDF file:

`pdf-parser --type={{/Font}} {{path/to/file.pdf}}`

- Search for strings in indirect objects:

`pdf-parser --search={{search_string}} {{path/to/file.pdf}}`
