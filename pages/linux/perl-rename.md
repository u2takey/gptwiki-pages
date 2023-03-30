# rename 
## chatgpt 
The "rename" command is used to rename files or directories in Linux. It allows users to change the names of one or more files or directories at once. 

The basic syntax of the rename command is as follows: 

```rename [options] 's/old_text/new_text/' file/s```

Here, "old_text" is the text that needs to be replaced, and "new_text" is the replacement text. The "s" flag indicates that the rename command is used to substitute the old text with the new one. 

Some of the options that can be used with the rename command are: 

- -v or --verbose: displays a list of files that have been renamed.
- -n or --no-action: displays the list of files that will be renamed, but does not actually rename them.
- -f or --force: forces the rename command to overwrite any existing files with the same name.

Example: 

Let's say we have a directory containing three files named file1.txt, file2.txt and file3.txt. If we want to rename all files that have the extension ".txt" to ".md", we can use the following command:

```rename 's/.txt$/.md/' *.txt```

This will rename all files from "file1.txt" to "file3.txt" to "file1.md" to "file3.md". 

Note: The rename command may vary slightly depending on the Linux distribution or version being used. 

## tldr 
 
> Rename multiple files.
> NOTE: this page refers to the command from the `perl-rename` Arch Linux package.
> More information: <https://manned.org/rename>.

- Rename files using a Perl Common Regular Expression (substitute 'foo' with 'bar' wherever found):

`rename {{'s/foo/bar/'}} {{*}}`

- Dry-run - display which renames would occur without performing them:

`rename -n {{'s/foo/bar/'}} {{*}}`

- Force renaming even if the operation would remove existing destination files:

`rename -f {{'s/foo/bar/'}} {{*}}`

- Convert filenames to lower case (use `-f` in case-insensitive filesystems to prevent "already exists" errors):

`rename 'y/A-Z/a-z/' {{*}}`

- Replace whitespace with underscores:

`rename 's/\s+/_/g' {{*}}`
