# jc 
## chatgpt 
As an AI language model, I'm assuming you are referring to the `jc` command that is commonly used in Unix-like operating systems. The `jc` command is a command-line utility that is used to convert complex JSON strings into formatted and more readable output. 

Here's an explanation of the various parts of the `jc` command:

`jc` - This is the command itself. It is used to convert JSON strings into more readable output.

`<JSON string>` - This is the JSON string that you want to convert. It can either be a string stored in a file or passed as an argument via the command line.

`-p` - This is an optional flag that tells `jc` to pretty-print the output with indentation and line breaks.

`-r` - This is another optional flag that tells `jc` to remove unnecessary whitespace from the output.

`-l` - This is yet another optional flag that tells `jc` to print the output in a "less" pager. This is useful when dealing with long JSON strings.

Overall, the `jc` command is a handy utility to use when working with JSON strings, as it can help you make sense of complex JSON data and debug issues with your JSON code. 

## tldr 
 
> A utility to convert the output of multiple commands to JSON.
> More information: <https://github.com/kellyjonbrazil/jc>.

- Convert command output to JSON via pipe:

`{{ifconfig}} | jc {{--ifconfig}}`

- Convert command output to JSON via magic syntax:

`jc {{ifconfig}}`

- Output pretty JSON via pipe:

`{{ifconfig}} | jc {{--ifconfig}} -p`

- Output pretty JSON via magic syntax:

`jc -p {{ifconfig}}`
