# ebook-convert 
## chatgpt 
The `ebook-convert` command is a command-line tool that is widely used in various ebook-related tasks. It is a part of the Calibre ebook management software and can be used to convert between different ebook formats, modify ebook metadata, and much more. Here is a detailed explanation of the command:

`ebook-convert` command structure:
```
ebook-convert input_file output_file [options]
```
- `input_file`: The path to the ebook file that you want to convert or modify.
- `output_file`: The path where the converted or modified ebook file will be saved.
- `[options]`: Optional flags or parameters that you can use to customize the conversion process.

Some of the most commonly used options in the `ebook-convert` command are:

- `--input-format`: Specifies the input ebook format. If not specified, Calibre tries to automatically detect the correct format.
- `--output-format`: Specifies the output ebook format. If not specified, Calibre tries to convert the input format to the best possible output format based on the input file type.
- `--title`: Sets the title of the ebook.
- `--author`: Sets the author name(s) of the ebook.
- `--publisher`: Sets the publisher of the ebook.
- `--language`: Sets the language of the ebook file.
- `--help`: Displays a list of available options.

Example usage:
```
ebook-convert my_book.epub my_book.mobi --output-format mobi --title "My Awesome Book" --author "John Doe" --publisher "My Publisher"
```
This command will convert the `my_book.epub` file to `my_book.mobi`, set the title to "My Awesome Book", author to "John Doe", and publisher to "My Publisher". 

Note: The `ebook-convert` command requires Calibre to be installed on your system. 

## tldr 
 
> Can be used to convert e-books between common formats, e.g. PDF, EPUB and MOBI.
> Part of the Calibre e-book library tool.
> More information: <https://manual.calibre-ebook.com/generated/en/ebook-convert.html>.

- Convert an e-book into another format:

`ebook-convert {{path/to/input_file}} {{output_file}}`

- Convert Markdown or HTML to e-book with TOC, title and author:

`ebook-convert {{path/to/input_file}} {{output_file}} --level1-toc="//h:h1" --level2-toc="//h:h2" --level3-toc="//h:h3" --title={{title}} --authors={{author}}`
