# rename 
## chatgpt 
The rename command is used to rename files and directories in Linux/Unix systems. It is also known as the "Perl rename" command because it uses Perl's regular expressions to match and manipulate filenames. 

Syntax: 
rename [options] expression replacement file...

Options: 
- -n or --no-act: Only shows the list of files to be renamed without actually renaming them. 
- -v or --verbose: Displays detailed output of the renaming process. 
- -f or --force: Forces the renaming of a file even if a file with the same name exists. 

Expression: This is the Perl regular expression that will be used to match the part of the file name that needs to be renamed. 

Replacement: This is the new name that will replace the part of the file name defined in the expression. 

File: The files or directories that need to be renamed. 

Example: 
Suppose you have a directory containing files named "file1.txt", "file2.txt", and "file3.txt". You want to rename all of them, replacing "file" with "newfile". 

Command: 
rename 's/file/newfile/' *.txt 

Explanation: 
- "s/file/newfile/" is the expression that specifies that all instances of "file" in the file name should be replaced with "newfile". 
- "*.txt" indicates that this command should be applied to all files ending with ".txt". 

The result will be files named "newfile1.txt", "newfile2.txt", and "newfile3.txt". 

## tldr 
 
> Rename multiple files.
> NOTE: this page refers to the command from the `prename` Fedora package.
> More information: <https://manned.org/man/prename>.

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
