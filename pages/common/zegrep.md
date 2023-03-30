# zegrep 
## chatgpt 
zegrep is a command that is used to search for a pattern or regular expression in compressed files. It is essentially the same as the grep command, but specifically designed to work with compressed files.

The zegrep command searches for the specified pattern in files that have been compressed with gzip, bzip2, or xz. It can be used to search for a pattern in a single file or in multiple files at once.

The general syntax for the zegrep command is as follows:

zegrep [OPTIONS] PATTERN [FILE...]

Where OPTIONS are any additional options that you want to pass to the command, PATTERN is the regular expression or pattern that you want to search for, and FILE... represents the list of files that you want to search.

Some of the commonly used options available with the zegrep command are:

-i: Ignores case sensitivity while searching.

-v: Displays all lines that do not match the pattern.

-n: Shows the line number of matched lines.

-c: Displays the count of matched lines.

For example, to search for the word "example" in a compressed file named "testfile.gz", you can use the following command:

zegrep "example" testfile.gz

Similarly, to search for the word "example" in all compressed files in the current directory, you can use the following command:

zegrep "example" *.gz

Overall, zegrep is a useful command for quickly searching for patterns in compressed files without having to decompress them first. 

## tldr 
 
> Find extended regular expression patterns in compressed files using `egrep`.
> More information: <https://www.unix.com/man-page/freebsd/1/zegrep/>.

- Search for extended regular expressions (supporting `?`, `+`, `{}`, `()` and `|`) in a compressed file (case-sensitive):

`zegrep "{{search_pattern}}" {{path/to/file}}`

- Search for extended regular expressions (supporting `?`, `+`, `{}`, `()` and `|`) in a compressed file (case-insensitive):

`zegrep --ignore-case "{{search_pattern}}" {{path/to/file}}`

- Search for lines that do not match a pattern:

`zegrep --invert-match "{{search_pattern}}" {{path/to/file}}`

- Print file name and line number for each match:

`zegrep --with-filename --line-number "{{search_pattern}}" {{path/to/file}}`

- Search for lines matching a pattern, printing only the matched text:

`zegrep --only-matching "{{search_pattern}}" {{path/to/file}}`

- Recursively search files in a compressed file for a pattern:

`zegrep --recursive "{{search_pattern}}" {{path/to/file}}`
