# phpcpd 
## chatgpt 
phpcpd is a command line tool that detects copy/paste code in PHP projects. When executed in the command line, phpcpd scans the specified directory or file, identifies duplicated code blocks, and outputs a report highlighting each detected instance of duplicated code.

Here is the syntax for running phpcpd:

```
phpcpd [options] path/to/directory-or-file
```

The options available for phpcpd include:

- `--version` - Displays the current version of phpcpd
- `--help` - Displays the list of available options and commands
- `--min-lines` - Sets the minimum size of duplicated code blocks (default is 5)
- `--min-tokens` - Sets the minimum number of duplicated lines in a block (default is 70)
- `--exclude` - Excludes specified directories or files from being scanned for duplicated code
- `--names` - Only scans files that match the specified name pattern (e.g. "*.php")

After executing phpcpd, it will output a report that shows the filename, the starting line number, the number of lines, and number of tokens for each instance of duplicated code. It also calculates the similarity percentage of the block.

The phpcpd tool is useful for identifying copy/paste code and can help improve the quality of code by reducing redundancy and improving maintainability. 

## tldr 
 
> A copy and paste detector for PHP code.
> More information: <https://github.com/sebastianbergmann/phpcpd>.

- Analyze duplicated code for a specific file or directory:

`phpcpd {{path/to/file_or_directory}}`

- Analyze using fuzzy matching for variable names:

`phpcpd --fuzzy {{path/to/file_or_directory}}`

- Specify a minimum number of identical lines (defaults to 5):

`phpcpd --min-lines {{number_of_lines}} {{path/to/file_or_directory}}`

- Specify a minimum number of identical tokens (defaults to 70):

`phpcpd --min-tokens {{number_of_tokens}} {{path/to/file_or_directory}}`

- Exclude a directory from analysis (must be relative to the source):

`phpcpd --exclude {{path/to/excluded_directory}} {{path/to/file_or_directory}}`

- Output the results to a PHP-CPD XML file:

`phpcpd --log-pmd {{path/to/log_file}} {{path/to/file_or_directory}}`
