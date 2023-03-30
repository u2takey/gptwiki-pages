# ed 
## chatgpt 
Ed is a command-line text editor that is used to create, edit and manipulate text files. It is a basic line-oriented text editor that is very simple to use and is popular among Unix and Linux users.

The general syntax of the ed command is:

```
ed [options] [filename]
```

Some of the commonly used options of the ed command are:

- `-p`: This option sets the prompt string that the user sees when using the ed editor.
- `-s`: This option suppresses the diagnostics message.
- `-v`: This option activates the verbose mode, which displays additional information during editing.

Once you launch the ed editor, you will be presented with a `:` prompt. This indicates that the editor is ready to take in commands. You can then enter commands to perform various operations.

Some of the commonly used commands in the ed editor are:

- `a`: This command is used to append text to the existing text in the file.
- `c`: This command is used to change the text in the file.
- `d`: This command is used to delete a line or a range of lines from the file.
- `e`: This command is used to open a new file for editing.
- `f`: This command is used to display the name of the file currently being edited.
- `p`: This command is used to print one or more lines of text from the file.
- `q`: This command is used to exit the ed editor.

To use the ed editor, you need to be familiar with its commands and their usage. It is a powerful yet simple text editor that can be used to quickly edit text files on the command line. 

## tldr 
 
> The original Unix text editor.
> See also: `awk`, `sed`.
> More information: <https://www.gnu.org/software/ed/manual/ed_manual.html>.

- Start an interactive editor session with an empty document:

`ed`

- Start an interactive editor session with an empty document and a specific prompt:

`ed --prompt='> '`

- Start an interactive editor session with user-friendly errors:

`ed --verbose`

- Start an interactive editor session with an empty document and without diagnostics, byte counts and '!' prompt:

`ed --quiet`

- Start an interactive editor session without exit status change when command fails:

`ed --loose-exit-status`

- Edit a specific file (this shows the byte count of the loaded file):

`ed {{path/to/file}}`

- Replace a string with a specific replacement for all lines:

`,s/{{regular_expression}}/{{replacement}}/g`
