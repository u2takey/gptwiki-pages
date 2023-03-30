# findstr 
## chatgpt 
The `findstr` command is a Windows command line utility that searches for a specific string or text pattern in one or more files. It is used to extract lines of text that match a certain pattern, and can also be used to exclude lines that do not match the pattern.

Here are some important details to consider when using the `findstr` command:

- Syntax: `findstr [options] [string] [filename]`

- Options: There are various options, flags and switches that can be used with the `findstr` command to modify its behavior. For example, the `/C` switch is used to specify the search string, while the `/B` switch indicates that the search should be constrained to the beginning of each line.

- String: This is the text string or regular expression pattern that you want to search for within the specified file(s).

- Filename: This is the name of the file(s) you want to search within. You can use wildcards to specify multiple files, such as `*.txt` to search all .txt files in the current directory.

- Usage: Once you know what you want to search for and which file(s) to search within, you can use the `findstr` command to locate the matching lines. For example, `findstr /C:"hello" myfile.txt` will find and display all lines in `myfile.txt` that contain the word "hello". Similarly, `findstr /V "goodbye" myfile.txt` will display all lines in `myfile.txt` that do not contain the word "goodbye".

Overall, the `findstr` command is a very useful tool for Windows users who need to locate and extract specific information from text files. 

## tldr 
 
> Find specified text within one or more files.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/findstr>.

- Find space-separated string(s) in all files:

`findstr "{{query}}" *`

- Find space-separated string(s) in a piped command's output:

`{{dir}} | findstr "{{query}}"`

- Find space-separated string(s) in all files recur[s]ively:

`findstr /s "{{query}}" *`

- Find strings using a case-insensitive search:

`findstr /i "{{query}}" *"`

- Find strings in all files using regular expressions:

`findstr /r "{{expression}}" *`

- Find a literal string (containing spaces) in all text files:

`findstr /c:"{{query}}" *.txt`

- Display the line number before each matching line:

`findstr /n "{{query}}" *`

- Display only the filenames that contain a match:

`findstr /m "{{query}}" *`
