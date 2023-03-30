# weasyprint 
## chatgpt 
WeasyPrint is a command-line tool that helps in generating PDF documents from HTML and CSS. It is written in Python programming language and uses the powerful webkit rendering engine.

To use WeasyPrint, simply type in the command "weasyprint" followed by the name of the HTML file you want to convert to PDF document. You can also specify additional options like page size, output directory, and CSS stylesheet files.

For example, the basic syntax of WeasyPrint command would be:

weasyprint [OPTIONS] INPUT_FILE [OUTPUT_FILE]

Here, options can be any additional parameters you want to include, like "–page-size A4", which sets the size of the output page to A4. INPUT_FILE is the name of the HTML file you want to convert, and OUTPUT_FILE is the name of the generated PDF file.

Other useful options for WeasyPrint command include:

- –quiet: suppresses all output messages except errors.
- –base-url: sets the base URL for resolving relative links and assets.
- –background-color: sets the background color of the output page.
- –html-encoding: sets the character encoding for the input HTML file.

Overall, WeasyPrint is a powerful command-line tool that helps in creating PDF documents from HTML and CSS files in a simple and efficient manner. 

## tldr 
 
> Render HTML to PDF or PNG.
> More information: <https://weasyprint.org/>.

- Render an HTML file to PDF:

`weasyprint {{path/to/input.html}} {{path/to/output}}.pdf`

- Render an HTML file to PNG, including an additional user stylesheet:

`weasyprint {{path/to/input.html}} {{path/to/output}}.png --stylesheet {{path/to/stylesheet.css}}`

- Output additional debugging information when rendering:

`weasyprint {{path/to/input.html}} {{path/to/output}}.pdf --verbose`

- Specify a custom resolution when outputting to PNG:

`weasyprint {{path/to/input.html}} {{path/to/output}}.png --resolution {{300}}`

- Specify a base URL for relative URLs in the input HTML file:

`weasyprint {{path/to/input.html}} {{path/to/output}}.png --base-url {{url_or_filename}}`
