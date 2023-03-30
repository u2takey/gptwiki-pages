# fossil add 
## chatgpt 
The `fossil add` command is used in the Fossil version control system to stage new files or changes to existing files for the next commit. When you create a new file or make changes to an existing file, the changes are initially stored in the working directory. However, to include these changes in the next commit, you must first add them to the staging area using the `add` command.

The syntax for the `fossil add` command is as follows:

```
fossil add <filename>
```
Here, `<filename>` is the name of the file that you want to add to the staging area.

You can also use the `fossil add` command with certain flags to perform additional actions:

- `-v`: Shows a verbose output of the added files.
- `-f`: Forces the addition of the file, even if Fossil believes the file has not changed.

After you have added the files to the staging area using the `fossil add` command, you can then commit the changes using the `fossil commit` command. 

## tldr 
 
> Put files or directories under Fossil version control.
> More information: <https://fossil-scm.org/home/help/add>.

- Put a file or directory under version control, so it will be in the current checkout:

`fossil add {{path/to/file_or_directory}}`

- Remove all added files from the current checkout:

`fossil add --reset`
