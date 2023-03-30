# peco 
## chatgpt 
peco is a command-line tool used for interactive filtering and selection of text. It takes a list of input items (typically obtained by piping in data from another command) and presents them in a dynamic, searchable user interface. The user can then interactively filter the list using regular expressions (regex) or simple text search, and select one or multiple items from the filtered list.

The peco command can be used in different ways, depending on the context. For example, you might use it to filter and select files in a directory, to select from a list of running processes, to choose from a list of available options, or to search and select items from a large text file.

Here's an example of how to use peco with a simple list of numbers:

    $ echo "1\n2\n3\n4\n5" | peco

This will present you with a searchable interface, where you can type a regex or text search term to filter the list of numbers. For example, typing "3" will highlight the number 3 in the list. You can then select the highlighted item (in this case, the number 3) by pressing Enter.

peco supports multiple selection modes, including single and multiple selections, and different key bindings for selection, filtering, and navigation. For more information on how to use peco, you can consult the official documentation or run "peco --help" for a list of available options and usage instructions. 

## tldr 
 
> Interactive filtering tool.
> More information: <https://github.com/peco/peco>.

- Start peco on all files in the specified directory:

`find {{path/to/directory}} -type f | peco`

- Start peco for running processes:

`ps aux | peco`

- Start peco with a specified query:

`peco --query "{{query}}"`
