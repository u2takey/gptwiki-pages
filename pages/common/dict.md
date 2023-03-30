# dict 
## chatgpt 
The "dict" command is not a standard command in the Unix or Linux operating system. However, it is a command that can be installed on some systems and is typically used to access a dictionary or thesaurus from the command line.

When the "dict" command is used, it presents a command-line interface where a user can enter a word or phrase they want to look up. The command then searches the dictionary or thesaurus database for any matches and displays the results.

The "dict" command typically uses a database of words and their definitions or synonyms, which can be installed separately from the command itself. Some systems may also allow users to install multiple databases, allowing them to search through different dictionaries or thesauruses.

Overall, the "dict" command can be a useful tool for quick word and phrase lookups from the command line, especially for users who prefer to work without leaving the terminal. 

## tldr 
 
> Command line dictionary using the DICT protocol.
> More information: <https://github.com/cheusov/dictd>.

- List available databases:

`dict -D`

- Get information about a database:

`dict -i {{database_name}}`

- Look up a word in a specific database:

`dict -d {{database_name}} {{word}}`

- Look up a word in all available databases:

`dict {{word}}`

- Show information about the DICT server:

`dict -I`
