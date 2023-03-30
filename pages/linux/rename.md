# rename 
## chatgpt 
The rename command is used to rename files and directories. It is a Linux/Unix command and can be used in the terminal. The syntax of the rename command is as follows: 

rename [options] [expression] [replacement] [file...]

Options:
- -v, --verbose: print the names of files that have been renamed.
- -n, --nono: test run only, do not make any actual file changes.
- -f, --force: overwrite existing files without asking.

Expression: This is the regular expression used to select the file or files to be renamed.

Replacement: This is the replacement string used to rename the selected files.

File...: This is the name of the file or files to be renamed.

For example, if you want to rename all files with the extension ".txt" to have a ".dat" extension, you could use the following command:

rename 's/.txt$/.dat/' *.txt

This command will rename all files with the ".txt" extension to have a ".dat" extension. The regular expression ".txt$" matches any file with the ".txt" extension, and the replacement string ".dat" replaces that extension with ".dat".

Note that the rename command is a powerful tool for batch renaming files, but it can also be dangerous if used incorrectly. It is always recommended to test the command with the -n option to ensure that it will behave as expected before using it with the -f option to make any actual file changes. 

## tldr 
 
> Rename multiple files.
> NOTE: this page refers to the command from the `util-linux` package.
> For the Perl version, see `file-rename` or `perl-rename`.
> Warning: This command has no safeguards and will overwrite files without prompting.
> More information: <https://manned.org/rename>.

- Rename files using simple substitutions (substitute 'foo' with 'bar' wherever found):

`rename {{foo}} {{bar}} {{*}}`

- Dry-run - display which renames would occur without performing them:

`rename -vn {{foo}} {{bar}} {{*}}`

- Do not overwrite existing files:

`rename -o {{foo}} {{bar}} {{*}}`

- Change file extensions:

`rename {{.ext}} {{.bak}} {{*.ext}}`

- Prepend "foo" to all filenames in the current directory:

`rename {{''}} {{'foo'}} {{*}}`

- Rename a group of increasingly numbered files zero-padding the numbers up to 3 digits:

`rename {{foo}} {{foo00}} {{foo?}} && rename {{foo}} {{foo0}} {{foo??}}`
