# unison 
## chatgpt 
Unison is a file synchronization application that allows two or more directories to be kept in sync with each other. It works by comparing the contents of two different directories and copying over any differences to ensure that both directories remain identical.

The syntax for using the unison command is as follows:

```
unison [options] [path1] [path2]
```

Where `[options]` are any additional command line parameters that can be passed to the unison application, and `[path1]` and `[path2]` are the two directories that need to be kept in sync.

Some of the key options that can be used with the unison command include:

- `-batch`: Runs unison in batch mode, which means it will not prompt the user for input during the synchronization process.
- `-ignore`: Allows you to specify a pattern or regular expression for files that should be ignored during the synchronization process.
- `-times`: Preserves the timestamps of files and directories during the synchronization process.

In addition, there are several other options that can be used to control various aspects of the synchronization process, such as how conflicts are handled and how files are renamed or moved.

Overall, the unison command is a powerful and flexible tool for keeping multiple directories in sync with each other, and can be used in a wide range of applications such as software development, backup and data migration. 

## tldr 
 
> Bidirectional file synchronisation tool.
> More information: <https://www.cis.upenn.edu/~bcpierce/unison/download/releases/stable/unison-manual.html>.

- Sync two directories (creates log first time these two directories are synchronized):

`unison {{path/to/directory_1}} {{path/to/directory_2}}`

- Automatically accept the (non-conflicting) defaults:

`unison {{path/to/directory_1}} {{path/to/directory_2}} -auto`

- Ignore some files using a pattern:

`unison {{path/to/directory_1}} {{path/to/directory_2}} -ignore {{pattern}}`

- Show documentation:

`unison -doc {{topics}}`
