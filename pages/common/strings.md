# strings 
## chatgpt 
The Linux command "strings" is used to extract printable strings from binary files. It scans the specified binary file and prints all the ASCII strings present in it. By default, it looks for strings that are at least 4 characters long, but this length can be adjusted using the command-line options. 

The syntax for the strings command is as follows:

```strings [options] filename```

Some of the commonly used options are:

- -n: Specifies the minimum length of the strings to be output. For example, -n 10 will print only strings that are at least 10 characters long. The default value is 4.
- -a: Prints all strings in the file, including those that are fewer than the minimum length specified with -n.
- -e: Specifies the character encoding of the binary file. The default is ASCII, but other options include big5, utf16, and utf32.
- -t: Prints the offset of each string within the file.

By default, strings outputs all of the printable strings in a file, but it can be useful to filter out certain types of strings. For example, you may want to exclude certain words or exclude strings that begin with certain characters. This can be achieved using standard Unix commands such as grep or awk, piped together with the strings command. 

The strings command is commonly used for analyzing binary files, particularly for extracting sensitive or hidden information from them. It can also be used for detecting or analyzing malware, as it may uncover hidden code or commands that have been embedded within a file. 

## tldr 
 
> Find printable strings in an object file or binary.
> More information: <https://manned.org/strings>.

- Print all strings in a binary:

`strings {{path/to/file}}`

- Limit results to strings at least *length* characters long:

`strings -n {{length}} {{path/to/file}}`

- Prefix each result with its offset within the file:

`strings -t d {{path/to/file}}`

- Prefix each result with its offset within the file in hexadecimal:

`strings -t x {{path/to/file}}`
