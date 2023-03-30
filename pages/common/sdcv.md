# sdcv 
## chatgpt 
The command 'sdcv' stands for 'StarDict Console Version'. This is a command-line utility used to fetch and display word definitions and translations from various dictionaries in StarDict format.

The 'sdcv' command takes one or more arguments, which are the words you want to search for. You can use several options to customize the output of the command. Some of the most commonly used options include:

- -n: Specify the number of definitions to display.
- -a: Show all available dictionaries.
- -d: Specify one or more dictionaries to use for the search.
- -t: Translation mode. Display translation of the word into other languages available in the dictionary.

Usage examples:

- sdcv hello: This command will search for the definition of the word 'hello' in all available dictionaries.
- sdcv -n 2 goodbye: This command will search for the definition of the word 'goodbye' and will display only the first two results.
- sdcv -d Oxford-LDOCE some: This command will search for the definition of the word 'some' using the Oxford-LDOCE dictionary.
- sdcv -t eng-rus car: This command will translate the word 'car' from English to Russian. 

## tldr 
 
> StarDict, a command-line dictionary client.
> Dictionaries are provided separately from the client.
> More information: <https://manned.org/sdcv>.

- Start sdcv interactively:

`sdcv`

- List installed dictionaries:

`sdcv --list-dicts`

- Display a definition from a specific dictionary:

`sdcv --use-dict {{dictionary_name}} {{search_term}}`

- Look up a definition with a fuzzy search:

`sdcv {{search_term}}`

- Look up a definition with an exact search:

`sdcv --exact-search {{search_term}}`

- Look up a definition and format the output as JSON:

`sdcv --json {{search_term}}`

- Search for dictionaries in a specific directory:

`sdcv --data-dir {{path/to/directory}} {{search_term}}`
