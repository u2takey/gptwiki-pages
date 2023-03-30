# asciidoctor 
## chatgpt 
Asciidoctor is a command-line tool that converts AsciiDoc documents into various formats, including HTML, PDF, and EPUB. AsciiDoc is a plain-text document format that uses simple markup syntax to create rich documents. The asciidoctor command is used to run the Asciidoctor tool on a specified AsciiDoc file or directory. 

The basic syntax of the asciidoctor command is as follows:

```
asciidoctor [OPTIONS] FILE
```

Where:

- `OPTIONS` are optional command-line arguments that configure the Asciidoctor tool's behavior, such as specifying the output format or customizing the document's appearance.
- `FILE` is the path to the AsciiDoc file or directory that should be processed.

By default, the asciidoctor command will generate an HTML document from the specified AsciiDoc file. However, you can use various command-line options to customize the output, such as generating a different format, applying custom stylesheets, or controlling the document's metadata.

Here are some common examples of using the asciidoctor command:

- To convert a single AsciiDoc file to HTML:

  ```
  asciidoctor hello.adoc
  ```

- To generate a PDF document from an AsciiDoc file:

  ```
  asciidoctor -r asciidoctor-pdf -b pdf hello.adoc
  ```

- To apply a custom stylesheet:

  ```
  asciidoctor -a stylesheet=my-styles.css hello.adoc
  ```

- To control the document's metadata:

  ```
  asciidoctor -a author="John Doe" -a date="2022-01-01" hello.adoc
  ```

Overall, the asciidoctor command is a powerful tool for converting AsciiDoc documents to various formats and customizing the output to meet your needs. 

## tldr 
 
> A processor that converts AsciiDoc files to a publishable format.
> More information: <https://docs.asciidoctor.org>.

- Convert a specific `.adoc` file to HTML (the default output format):

`asciidoctor {{path/to/file.adoc}}`

- Convert a specific `.adoc` file to HTML and link a CSS stylesheet:

`asciidoctor -a stylesheet={{path/to/stylesheet.css}} {{path/to/file.adoc}}`

- Convert a specific `.adoc` file to embeddable HTML, removing everything except the body:

`asciidoctor --embedded {{path/to/file.adoc}}`

- Convert a specific `.adoc` file to a PDF using the `asciidoctor-pdf` library:

`asciidoctor --backend={{pdf}} --require={{asciidoctor-pdf}} {{path/to/file.adoc}}`
