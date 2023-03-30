# psgrep 
## chatgpt 
Sorry, as an AI language model, I am not familiar with a command called "psgrep". It is possible that it is a custom or non-standard command, or it may be a typo or misspelling of a similar command, such as "ps aux | grep" or "pgrep". Can you provide more context or information about the command? 

## tldr 
 
> Search running processes with `grep`.
> More information: <https://jvz.github.io/psgrep>.

- Find process lines containing a specific string:

`psgrep {{process_name}}`

- Find process lines containing a specific string, excluding headers:

`psgrep -n {{process_name}}`

- Search using a simplified format (PID, user, command):

`psgrep -s {{process_name}}`
