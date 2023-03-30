# jdupes 
## chatgpt 
jdupes is a command line utility tool used for finding and eliminating duplicate files on a computer's file system. The command works by analyzing the contents of each file and comparing them, and then marking the duplicates for further actions like deletion, hard linking, or moving to another location.

To use jdupes, it is necessary to open the terminal, navigate to the directory or folder containing the files to be searched and run the command, which is simply "jdupes" followed by several additional arguments:

1. `-r` or `--recurse`: this argument will make jdupes search for duplicates in all subdirectories of the specified folder.

2. `-d` or `--delete`: this argument will delete all the duplicates found, retaining only one copy of each file. Note that this action is permanent and cannot be undone. 

3. `-n` or `--noempty`: this argument will skip empty files as it is assumed that empty files cannot have duplicates.

4. `-H` or `--hardlink`: this argument will create hard links to duplicate files instead of deleting them. This is a way to save space on a file system without deleting files.

5. `-m` or `--summarize`: this argument will provide a brief summary of the duplicates found without listing every identical file. 

Overall, the jdupes command is a useful tool for finding and deleting duplicate files on a computer. However, as always, it is recommended to back up all important data before using any data-management tool. 

## tldr 
 
> A powerful duplicate file finder and an enhanced fork of fdupes.
> More information: <https://github.com/jbruchon/jdupes>.

- Search a single directory:

`jdupes {{path/to/directory}}`

- Search multiple directories:

`jdupes {{directory1}} {{directory2}}`

- Search all directories recursively:

`jdupes --recurse {{path/to/directory}}`

- Search directory recursively and let user choose files to preserve:

`jdupes --delete --recurse {{path/to/directory}}`

- Search multiple directories and follow subdirectores under directory2, not directory1:

`jdupes {{directory1}} --recurse: {{directory2}}`

- Search multiple directories and keep the directory order in result:

`jdupes -O {{directory1}} {{directory2}} {{directory3}}`
