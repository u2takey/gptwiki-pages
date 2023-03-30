# fc 
## chatgpt 
The "fc" command is a shell built-in command in Unix-like operating systems that is used to list, edit, and re-execute commands from the history of commands entered in the current shell session.

The basic syntax of the "fc" command is as follows:

fc [options] [first [last]]

Here, the "options" parameter is an optional list of flags that change the behavior of the command. The "first" parameter is also optional and specifies the first command to include in the range of commands to be processed. The "last" parameter is also optional and specifies the last command to include in the range of commands to be processed.

Some of the commonly used options with the "fc" command are:

- -l: This option lists the commands in the history buffer. If no range of commands is specified, it lists all the commands.
- -e: This option launches the default text editor to edit the selected command(s) before executing them. By default, the "vi" editor is used, but this can be changed by setting the $FCEDIT or $EDITOR environment variables.
- -n: This option suppresses the execution of the selected command(s) after they have been edited, allowing the user to review and save them without executing them.
- -r: This option reverses the order of the selected commands, executing them in reverse order from the most recent to the oldest.

For example, to re-execute the last command in the history buffer using the "fc" command, you can use the following command:

fc -s

Here, the "-s" option specifies to re-execute the most recent command in the history buffer. 

## tldr 
 
> Compare the differences between two files or sets of files.
> Use wildcards (*) to compare sets of files.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/fc>.

- Compare 2 specified files:

`fc {{path\to\file1}} {{path\to\file2}}`

- Perform a case-insensitive comparison:

`fc /c {{path\to\file1}} {{path\to\file2}}`

- Compare files as Unicode text:

`fc /u {{path\to\file1}} {{path\to\file2}}`

- Compare files as ASCII text:

`fc /l {{path\to\file1}} {{path\to\file2}}`

- Compare files as binary:

`fc /b {{path\to\file1}} {{path\to\file2}}`

- Disable tab-to-space expansion:

`fc /t {{path\to\file1}} {{path\to\file2}}`

- Compress whitespace (tabs and spaces) for comparisons:

`fc /w {{path\to\file1}} {{path\to\file2}}`
