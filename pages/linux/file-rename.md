# rename 
## chatgpt 
The `rename` command is used to rename files and directories in Linux or Unix operating system.

The syntax of the command is:

```
rename [options] 's/old-pattern/new-pattern/' files
```

Where:
- `[options]`: (Optional) Additional options that you can pass to the command.
- `s`: Indicates that we want to perform a substitution.
- `old-pattern`: The existing pattern or string that you want to replace.
- `new-pattern`: The new pattern or string that you want to replace the old pattern with.
- `files`: The name or pattern of the files or directories that you want to rename.

For example, to rename all files with the extension `.txt` to have the extension `.md`, you could use the following command:

```
rename 's/.txt$/.md/' *.txt
```

This command will replace the `.txt` extension with `.md` for all files in the current directory that end with `.txt`. Note that the `*` is used as a wildcard character to match any filename that ends with `.txt`.

Some common options that you can use with the `rename` command are:

- `-n` or `--dry-run`: This option will show you what the command would do without actually renaming any files.
- `-v` or `--verbose`: This option will print out each filename as it is being renamed. 

## tldr 
 
> Rename multiple files.
> NOTE: this page refers to the command from the `rename` Debian package.
> More information: <https://manned.org/file-rename>.

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
