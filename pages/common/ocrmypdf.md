# ocrmypdf 
## chatgpt 
OCRMYPDF is a command-line tool for adding OCR (Optical Character Recognition) text layer to PDF documents, which enables searching and copying of text from scanned PDFs. The command has the following syntax:

ocrmypdf [OPTIONS] INPUT_FILE [OUTPUT_FILE]

OPTIONS:
- -l, --language: The language(s) to use for OCR. Multiple languages can be specified as a comma-separated list. By default, English is used.
- -c, --output-type: The output format of the OCR text layer. The default is hOCR (HTML-based OCR).
- -t, --deskew: Apply automatic deskewing to the document before OCR.
- -d, --debug: Enables debug mode and logs debugging messages to the console.
- -v, --version: Prints the version number of ocrmypdf and exits.
- -h, --help: Prints the help message and exits.

INPUT_FILE: The path to the PDF file to be OCR'ed.

OUTPUT_FILE: The path to the resulting PDF file with the OCR text layer added. If not provided, it defaults to a file with the same name as the input file, but with '-ocr.pdf' appended.

Example usage:

To OCR a PDF file named 'example.pdf' with English language and save OCR'ed output as 'example-ocr.pdf':

ocrmypdf example.pdf example-ocr.pdf

To OCR a PDF file named 'example.pdf' with French and Spanish languages and save OCR'ed output as 'example-ocr.pdf':

ocrmypdf -l fra,spa example.pdf example-ocr.pdf

To OCR a PDF file named 'example.pdf' with automatic deskewing applied and save OCR'ed output as 'example-ocr.pdf':

ocrmypdf -t example.pdf example-ocr.pdf

Overall, ocrmypdf is a convenient and powerful tool for improving the accessibility and searchability of PDF documents with OCR. 

## tldr 
 
> Generate a searchable PDF or PDF/A from a scanned PDF or an image of text.
> More information: <https://ocrmypdf.readthedocs.io/en/latest/cookbook.html>.

- Create a new searchable PDF/A file from a scanned PDF or image file:

`ocrmypdf {{path/to/input_file}} {{path/to/output.pdf}}`

- Replace a scanned PDF file with a searchable PDF file:

`ocrmypdf {{path/to/file.pdf}} {{path/to/file.pdf}}`

- Skip pages of a mixed-format input PDF file that already contain text:

`ocrmypdf --skip-text {{path/to/input.pdf}} {{path/to/output.pdf}}`

- Clean, de-skew, and rotate pages of a poor scan:

`ocrmypdf --clean --deskew --rotate-pages {{path/to/input_file}} {{path/to/output.pdf}}`

- Set the metadata of the searchable PDF file:

`ocrmypdf --title "{{title}}" --author "{{author}}" --subject "{{subject}}" --keywords "{{keyword; key phrase; ...}}" {{path/to/input_file}} {{path/to/output.pdf}}`

- Display help:

`ocrmypdf --help`
