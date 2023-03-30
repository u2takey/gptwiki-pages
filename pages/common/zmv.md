# zmv 
## chatgpt 
zmv is a powerful command-line tool used to batch rename files and directories in UNIX and UNIX-like operating systems. It is an extension of the standard mv command and is used to mass-rename files and directories.

The zmv command works by using shell globbing patterns and regular expressions to search through a set of files and directories, and then renaming them according to a set of rules. Here are some of the key features of the zmv command:

1. Renaming Files and Directories: The zmv command can be used to rename files and directories by specifying a pattern and a replacement string. For example, the command:

   zmv '(*).txt' '$1.original.txt'

   will rename all files ending in ".txt" to ".original.txt".

2. Renaming Files/Directories Recursively: The zmv command can also recursively rename files and directories in a specified directory and all its subdirectories. For example, the command:

   zmv '(**/)(*).txt' '$1$2.original.txt'

   will rename all files ending in ".txt" in the current directory and all its subdirectories to ".original.txt".

3. Preview Mode: The zmv command has a preview mode which allows you to see what the command will do without actually renaming any files. This can be useful to check if the command is doing what you want it to do. For example, the command:

   zmv -n '(*).txt' '$1.original.txt'

   will show you what the command will do without actually renaming any files.

4. Dry Run or Simulation Mode: The zmv command has a dry run or simulation mode that can be very useful in making sure that the renaming operations you perform are safe and accurate. In this mode, the command only simulates what it would do without actually renaming any files or directories. To activate this mode, use the -S option.

5. Advanced Regular Expression Support: The zmv command supports advanced regular expressions using the Perl Compatible Regular Expression (PCRE) library. This allows you to use very powerful and complex regular expressions to perform renaming operations.

Overall, the zmv command provides a powerful and flexible way to batch rename files and directories in UNIX and UNIX-like operating systems. 

## tldr 
 
> Move or rename files matching a specified extended glob pattern.
> See also `zcp` and `zln`.
> More information: <http://zsh.sourceforge.net/Doc/Release/User-Contributions.html>.

- Move files using a regular expression-like pattern:

`zmv '{{(*).log}}' '{{$1.txt}}'`

- Preview the result of a move, without making any actual changes:

`zmv -n '{{(*).log}}' '{{$1.txt}}'`

- Interactively move files, with a prompt before every change:

`zmv -i '{{(*).log}}' '{{$1.txt}}'`

- Verbosely print each action as it's being executed:

`zmv -v '{{(*).log}}' '{{$1.txt}}'`
