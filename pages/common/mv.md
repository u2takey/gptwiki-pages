# mv 
## chatgpt 
The "mv" command is a Linux/Unix shell command used to move or rename files and directories. The full form of "mv" is "move". The basic syntax of the "mv" command is:

```
mv oldfile newfile
```

Here, "oldfile" is the name/path of the existing file or directory that you want to move or rename, and "newfile" is the new name/path that you want to assign to that file or directory. When you use the "mv" command with only two arguments, it simply renames the file or directory.

Examples:
- To move a file named "file1.txt" from the current directory to another directory "backup", the command would be:
```
mv file1.txt backup/
```
- To rename a file named "oldfile.txt" to "newfile.txt":
```
mv oldfile.txt newfile.txt
```
- To move a directory named "docs" from the current directory to another directory named "backup":
```
mv docs/ backup/
```
- To rename a directory named "olddir" to "newdir":
```
mv olddir/ newdir/
```
You can also use the "mv" command to move multiple files or directories at once by providing multiple arguments. 

## tldr 
 
> Move or rename files and directories.
> More information: <https://www.gnu.org/software/coreutils/mv>.

- Rename a file or directory when the target is not an existing directory:

`mv {{source}} {{target}}`

- Move a file or directory into an existing directory:

`mv {{source}} {{existing_directory}}`

- Move multiple files into an existing directory, keeping the filenames unchanged:

`mv {{source1}} {{source2}} {{source3}} {{existing_directory}}`

- Do not prompt for confirmation before overwriting existing files:

`mv -f {{source}} {{target}}`

- Prompt for confirmation before overwriting existing files, regardless of file permissions:

`mv -i {{source}} {{target}}`

- Do not overwrite existing files at the target:

`mv -n {{source}} {{target}}`

- Move files in verbose mode, showing files after they are moved:

`mv -v {{source}} {{target}}`
