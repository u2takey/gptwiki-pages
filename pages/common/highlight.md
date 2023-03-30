# highlight 
## chatgpt 
As an AI language model, I cannot tell which highlight command are you referring to. There are several possible commands or tools that may use the term "highlight". Could you please provide more context or information about the specific command you want me to explain? 

## tldr 
 
> Outputs syntax-highlighted source code to a variety of formats.
> More information: <http://www.andre-simon.de/doku/highlight/highlight.php>.

- Produce a complete HTML document from a source code file:

`highlight --out-format={{html}} --style {{theme_name}} --syntax {{language}} {{path/to/source_code}}`

- Produce an HTML fragment, suitable for inclusion in a larger document:

`highlight --out-format={{html}} --fragment --syntax {{language}} {{source_file}}`

- Inline the CSS styling in every tag:

`highlight --out-format={{html}} --inline-css --syntax {{language}} {{source_file}}`

- List all supported languages, themes, or plugins:

`highlight --list-scripts {{langs|themes|plugins}}`

- Print a CSS stylesheet for a theme:

`highlight --out-format={{html}} --print-style --style {{theme_name}} --syntax {{language}}] --stdout`
