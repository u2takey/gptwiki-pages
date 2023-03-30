# csslint 
## chatgpt 
CSSLint is a command-line tool used by web developers for checking Cascading Style Sheets (CSS) code quality. It helps identify potential errors, violations, and formatting inconsistencies.

The CSSLint command can be used in the terminal or command prompt to execute the tool. Once executed, it scans the CSS file and highlights any potential errors or warnings.

The command usage typically involves specifying the CSS file or directory to be scanned, and providing any additional options such as format or rule set selection.

For example, the syntax for scanning a CSS file with CSSLint might look something like this:

csslint file.css

This command would tell CSSLint to scan the file.css file for any potential errors or warnings.

CSSLint also allows for customization through configuration files that can specify which rules to enable or disable, or set specific formatting preferences.

Overall, CSSLint can be a helpful tool in identifying and improving CSS code quality, ensuring that web pages and applications are well-designed and optimized for performance. 

## tldr 
 
> A linter for CSS code.
> More information: <https://github.com/CSSLint/csslint/wiki/Command-line-interface>.

- Lint a single CSS file:

`csslint {{file.css}}`

- Lint multiple CSS files:

`csslint {{file1.css}} {{file2.css}} {{file3.css}}`

- List all possible style rules:

`csslint --list-rules`

- Specify certain rules as errors (which result in a non-zero exit code):

`csslint --errors={{errors,universal-selector,imports}} {{file.css}}`

- Specify certain rules as warnings:

`csslint --warnings={{box-sizing,selector-max,floats}} {{file.css}}`

- Specify certain rules to ignore:

`csslint --ignore={{ids,rules-count,shorthand}} {{file.css}}`
