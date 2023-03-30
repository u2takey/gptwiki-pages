# keep-header 
## chatgpt 
Unfortunately, without additional context, it is not possible to provide a comprehensive explanation of the command "keep-header." The term "keep-header" could potentially refer to a command in a specific programming language or software program, and its exact function and syntax would depend on the specific context in which it is being used. 

However, based on the term itself, "keep-header" may potentially be used in a data processing or analysis context. In this case, "keep-header" might be a command that specifies that the first row of a data file should be treated as the header row, and that this row should be preserved (i.e. "kept") when processing or analyzing the data. 

Again, without more information about the specific context in which "keep-header" is being used, it is difficult to provide a more detailed explanation of the command. 

## tldr 
 
> Keep first line untouched by a command, passing it directly to `stdout`.
> More information: <https://github.com/eBay/tsv-utils#keep-header>.

- Sort a file and keep the first line at the top:

`keep-header {{path/to/file}} -- sort`

- Output first line directly to `stdout`, passing the remainder of the file through the specified command:

`keep-header {{path/to/file}} -- {{command}}`

- Read from `stdin`, sorting all except the first line:

`cat {{path/to/file}} | keep-header -- {{command}}`

- Grep a file, keeping the first line regardless of the search pattern:

`keep-header {{path/to/file}} -- grep {{pattern}}`
