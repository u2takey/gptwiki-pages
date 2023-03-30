# fzf 
## chatgpt 
fzf is a command-line tool and a powerful command-line fuzzy finder. It is a popular tool used for text searches and helps users traverse file systems, run commands, search Github repositories, and much more efficiently. 

Fzf stands for "fuzzy finder," so the software is designed to find matches even if the user only provides a partial input for their search. It has several interesting features that make it a great tool for users who spend a lot of time working with the command line interface.

Some of the key features of fzf are:

1. Fuzzy Matching: With fuzzy matching, fzf can return results which approximate the search string the user inputs, though it might not be an exact match. This makes it easier for the user to navigate and search through large and complex directories.

2. Modular design: The architecture of fzf is highly modular, which makes it highly flexible and extensible. Users can take advantage of its APIs to build custom extensions and scripts.

3. Customizable Keybindings: fzf is highly configurable, which means users can customize keybindings according to their preferences.

4. Interactive Mode: With fzf, users have access to an interactive mode that makes it easier to navigate folders and search for files.

5. Speed: fzf is highly optimized for speed and leverages caching to reduce the time it takes to return search results.

Overall, fzf is an essential tool for anyone who spends a lot of time working with the command line interface. By adding powerful searching and navigation features, fzf helps users get the most out of their workflows, ultimately improving productivity and efficiency. 

## tldr 
 
> Command-line fuzzy finder.
> Similar to `sk`.
> More information: <https://github.com/junegunn/fzf>.

- Start fzf on all files in the specified directory:

`find {{path/to/directory}} -type f | fzf`

- Start fzf for running processes:

`ps aux | fzf`

- Select multiple files with `Shift + Tab` and write to a file:

`find {{path/to/directory}} -type f | fzf --multi > {{path/to/file}}`

- Start fzf with a specified query:

`fzf --query "{{query}}"`

- Start fzf on entries that start with core and end with either go, rb, or py:

`fzf --query "^core go$ | rb$ | py$"`

- Start fzf on entries that not match pyc and match exactly travis:

`fzf --query "!pyc 'travis"`
