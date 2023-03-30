# git sed 
## chatgpt 
I'm sorry, but there is no `git sed` command. 

`git` is a widely used version control system that allows users to track and manage changes made to source code and other files over time. 

`sed` is a command-line utility for parsing and transforming text. It can be used to edit files in place, search and replace text, and perform other text processing tasks. 

While `git` and `sed` can be used together in a variety of ways, there is no single command `git sed` that combines their functionality. If you have a specific use case in mind, please provide more details and I will be happy to assist you further. 

## tldr 
 
> Replace patterns in git-controlled files using sed.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-sed>.

- Replace the specified text in the current repository:

`git sed '{{find_text}}' '{{replace_text}}'`

- Replace the specified text and then commit the resulting changes with a standard commit message:

`git sed -c '{{find_text}}' '{{replace_text}}'`

- Replace the specified text, using regular expressions:

`git sed -f g '{{find_text}}' '{{replace_text}}'`

- Replace a specific text in all files under a given directory:

`git sed '{{find_text}}' '{{replace_text}}' -- {{path/to/directory}}`
