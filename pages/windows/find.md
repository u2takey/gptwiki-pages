# find 
## chatgpt 
The "find" command is used in Unix-based operating systems to search for files and directories within a specified directory hierarchy. It allows the user to specify a variety of search criteria, such as file name, type, size, owner, and modification time, and to execute commands on the files that match the criteria. 

To use the command, the user must specify the starting directory from which the search should begin. The most basic syntax for the command is:

```find [starting directory]```

For example, to search for all files and directories within the current working directory, the command would be:

```find .```

The dot (.) specifies the current directory as the starting point for the search. 

To narrow down the search, the user can add various options to specify the search criteria. Some common options include:

```-name [file name pattern]``` - Searches for files with a specific name, using wildcards if necessary (e.g. *.txt).

```-type [file type]``` - Searches for files of a specific type, such as f for regular files or d for directories.

```-size [file size]``` - Searches for files of a specific size, using units such as bytes (c), kilobytes (k), or megabytes (M).

```-user [file owner]``` - Searches for files owned by a specific user.

```-mtime [time period]``` - Searches for files modified within a specific time period, such as -1 for the past 24 hours or +7 for the past 7 days.

For example, the following command searches for all files with the extension .txt within the current working directory and its subdirectories:

```find . -name "*.txt"```

Once the search criteria have been specified, the user can also execute specific commands on the files that match the criteria. This is done by using the -exec option, followed by the command to be executed. For example, the following command searches for all files owned by the user "alice" and deletes them:

```find . -user alice -exec rm {} \;```

In this command, {} represents the list of files that match the search criteria, and \; indicates the end of the command to be executed. Note that it is important to use the backslash (\) before the semicolon (;) to ensure that the shell interprets it as part of the command, rather than as a separator between commands. 

## tldr 
 
> Find a specified string in one or more files.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/find>.

- Find lines that contain a specified string:

`find "{{string}}" {{path\to\file_or_directory}}`

- Display lines that do not contain the specified string:

`find "{{string}}" {{path\to\file_or_directory}} /v`

- Display the count of lines that contain the specified string:

`find "{{string}}" {{path\to\file_or_directory}} /c`

- Display line numbers with the list of lines:

`find "{{string}}" {{path\to\file_or_directory}} /n`
