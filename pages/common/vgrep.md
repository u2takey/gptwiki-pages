# vgrep 
## chatgpt 
Unfortunately, I cannot provide a detailed explanation of the command "vgrep" as it is not a standard Unix command or a commonly used command in any programming language. The command may be specific to a particular system or application. If you have more information about the context in which the command is being used, I may be able to provide more assistance. 

## tldr 
 
> A user friendly pager for grep.
> See also: `ugrep`, `rg`.
> More information: <https://github.com/vrothberg/vgrep>.

- Recursively search the current directory for a pattern and cache it:

`vgrep {{search_pattern}}`

- Display the contents of the cache:

`vgrep`

- Open the "4th" match from the cache in the default editor:

`vgrep --show {{4}}`

- Display a context of "3" lines for each match in the cache:

`vgrep --show=context{{3}}`

- Display the number of matches for each directory in the tree:

`vgrep --show=tree`

- Display the number of matches for each file in the tree:

`vgrep --show=files`

- Start an interactive shell with cached matches:

`vgrep --interactive`
