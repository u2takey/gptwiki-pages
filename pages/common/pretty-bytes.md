# pretty-bytes 
## chatgpt 
The `pretty-bytes` command is a utility used to convert a number of bytes into a human-readable format. It is commonly used in command-line interfaces to display the size of a file or directory in a user-friendly way. The command takes a number (in bytes) as input and returns a string containing the size in a readable format using units such as B, KB, MB, GB, TB, and PB. For example, if the input is 5000 bytes, the command will return the string "5 kB". This makes it easier for users to understand the size of the file or directory, especially when dealing with large amounts of data. The `pretty-bytes` command is often used in conjunction with other commands that output file or directory sizes, such as `du` or `ls`. 

## tldr 
 
> Convert bytes to a human-readable string.
> More information: <https://github.com/sindresorhus/pretty-bytes-cli>.

- Convert numeric bytes value to a human-readable string:

`pretty-bytes {{1337}}`

- Convert numeric bytes value from `stdin` to a human-readable string:

`echo {{1337}} | pretty-bytes`

- Display help and usage information:

`pretty-bytes --help`
