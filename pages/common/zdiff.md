# zdiff 
## chatgpt 
The `zdiff` command is used to compare and highlight the differences between compressed or gzip files. 

Syntax: `zdiff [OPTION]... FILE1 [FILE2]`

Here are some commonly used options with the `zdiff` command:

- `-c`, `--context`: Specifies how many lines of preceding and trailing context to include in output for each difference found. By default, this value is set to 3.
- `-u`, `--unified`: Similar to `-c`, but the output format is unified context format instead of the default context format.
- `-q`, `--brief`: Outputs only whether or not the files differ. No detailed difference report is given.
- `-i`, `--ignore-case`: Ignores case differences when comparing the files.
- `-w`, `--ignore-all-space`: Ignores all whitespace differences when comparing the files.
- `-B`, `--ignore-blank-lines`: Ignores all blank lines when comparing the files.

When executed, the `zdiff` command reads two compressed files and uses the `diff` command to compare the corresponding uncompressed files. The differences between the two files are displayed with `>` and `<` symbols to represent differences in the contents of the first and second files, respectively. An asterisk (*) is used to indicate that both files contain differences at that particular line number. 

Note that if the second file argument is omitted, `zdiff` will compare the contents of the first file to the uncompressed standard input. 

## tldr 
 
> Invoke `diff` on gzipped files.
> More information: <https://manned.org/zdiff>.

- Compare two files, uncompressing them if necessary:

`zdiff {{path/to/file1.gz}} {{path/to/file2.gz}}`

- Compare a file to a gzipped archive with the same name:

`zdiff {{path/to/file}}`
