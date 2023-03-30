# zfgrep 
## chatgpt 
zfgrep is a command used in Unix/Linux based operating system to search for a text pattern in files present in a compressed format. The command is a variant of the ‘grep’ command which is used to search for a pattern in un-compressed files.

The zfgrep command is used to search for a string or a pattern of characters in one or more compressed files without having to uncompress them first. The benefit of using this command is that it saves time compared to first uncompressing the file and then searching for the pattern.

The syntax of zfgrep command is as follows:

zfgrep [OPTIONS] PATTERN [FILE...]

Where OPTIONS are the additional options that can be specified, PATTERN is the pattern that needs to be searched and FILE is the compressed file where the search has to be performed.

Some of the commonly used options are:

- -i : This option ignores the case sensitivity of the pattern search. It means that both upper case and lower case characters will be searched.
- -r : This option recursively searches for the pattern in all the compressed files present in the current folder and its subfolders.
- -n : This option displays the line numbers where the pattern was found in the compressed files.

Here is an example of how to use the zfgrep command:

zfgrep -i "apple" fruits.gz

This command will search for the word “apple” in the compressed file “fruits.gz” while ignoring the case of the characters. The results will be displayed on the screen. 

## tldr 
 
> Matches fixed strings in possibly compressed files.
> Equivalent to `grep -F` with input decompressed first if necessary.
> More information: <https://manned.org/zfgrep>.

- Search for an exact string in a file:

`zfgrep {{search_string}} {{path/to/file}}`

- Count the number of lines that match the given string in a file:

`zfgrep --count {{search_string}} {{path/to/file}}`

- Show the line number in the file along with the matching lines:

`zfgrep --line-number {{search_string}} {{path/to/file}}`

- Display all lines except those that contain the search string:

`zfgrep --invert-match {{search_string}} {{path/to/file}}`

- List only filenames whose content matches the search string at least once:

`zfgrep --files-with-matches {{search_string}} {{path/to/file1 path/to/file2 ...}}`
