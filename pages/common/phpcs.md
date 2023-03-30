# phpcs 
## chatgpt 
"phpcs" is a command-line tool that stands for "PHP CodeSniffer". It is used for analyzing and checking PHP code conformity to coding standards. The tool uses a set of pre-defined coding standards that are applied to the code being analyzed. It highlights the parts of code that do not meet the coding standards and suggests possible changes to make the code better.

The syntax of the "phpcs" command is:

```
phpcs [options] [file or directory]
```

Some of the commonly used options with this command are:

- `-s`: This option shows the output in summary format.
- `-n`: This option will not print the warnings along with the report.
- `-p`: This option shows the progress of the analysis on the console.

The "file or directory" argument to the "phpcs" command is the path to the PHP files that need to be analyzed. If a directory is passed, the tool will scan all PHP files within that directory and its subdirectories.

Overall, the "phpcs" command is an essential tool for PHP developers as it helps ensure that the code they write is consistent and meets industry standards. 

## tldr 
 
> Tokenize PHP, JavaScript and CSS files to detect violations of a defined set of coding standards.
> More information: <https://github.com/squizlabs/PHP_CodeSniffer>.

- Sniff the specified directory for issues (defaults to the PEAR standard):

`phpcs {{path/to/directory}}`

- Display a list of installed coding standards:

`phpcs -i`

- Specify a coding standard to validate against:

`phpcs {{path/to/directory}} --standard {{standard}}`

- Specify comma-separated file extensions to include when sniffing:

`phpcs {{path/to/directory}} --extensions {{file_extension(s)}}`

- Specify the format of the output report (e.g. `full`, `xml`, `json`, `summary`):

`phpcs {{path/to/directory}} --report {{format}}`

- Set config variables to be used during the process:

`phpcs {{path/to/directory}} --config-set {{key}} {{value}}`

- A comma-separated list of files to load before processing:

`phpcs {{path/to/directory}} --bootstrap {{file(s)}}`

- Don't recurse into subdirectories:

`phpcs {{path/to/directory}} -l`
