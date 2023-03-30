# html5validator 
## chatgpt 
html5validator is a command-line tool that validates HTML5 files. When executed, the tool scans the specified HTML5 files and flags any errors or warnings encountered that are not compliant with the HTML5 specification.

The command syntax for html5validator is as follows:

```
html5validator [OPTIONS] [FILE(S)]
```

OPTIONS are optional parameters that can further refine the behavior of the tool. Some of the available options include:

- `--root` — change the root directory where the file(s) is located
- `--show-warnings` — include warnings in the output
- `--ignore-re` — ignore specific regular expressions for file paths
- `--match` — only validate files that match a specific regular expression

FILE(S) is a list of one or more HTML5 files to be validated. They can be specified as paths or as a glob pattern.

When executed, the html5validator tool will output any errors and warnings encountered during the validation process. If no errors or warnings are found, the output will be empty. In addition, html5validator exits with a 0 status code if there are no errors or warnings, and with a non-zero status code if there are any errors or warnings.

Overall, html5validator is a useful tool for ensuring that HTML5 files adhere to the HTML5 specification and are free of errors or potential issues. 

## tldr 
 
> A command-line tool for testing HTML5 validity.
> More information: <https://github.com/svenkreiss/html5validator>.

- Validate a specific file:

`html5validator {{path/to/file}}`

- Validate all HTML files in a specific directory:

`html5validator --root {{path/to/directory}}`

- Show warnings as well as errors:

`html5validator --show-warnings {{path/to/file}}`

- Match multiple files using a glob pattern:

`html5validator --root {{path/to/directory}} --match "{{*.html *.php}}"`

- Ignore specific directory names:

`html5validator --root {{path/to/directory}} --blacklist "{{node_modules vendor}}"`

- Output the results in a specific format:

`html5validator --format {{gnu|xml|json|text}} {{path/to/file}}`

- Output the log at a specific verbosity level:

`html5validator --root {{path/to/directory}} --log {{debug|info|warning}}`
