# sk 
## chatgpt 
I'm sorry, as an AI language model, I am not sure which command you are referring to with "sk". Please provide more information about the context or the operating system/environment in which the command is used. 

## tldr 
 
> Fuzzy finder written in Rust.
> Similar to `fzf`.
> More information: <https://github.com/lotabout/skim>.

- Start skim on all files in the specified directory:

`find {{path/to/directory}} -type f | sk`

- Start skim for running processes:

`ps aux | sk`

- Start skim with a specified query:

`sk --query "{{query}}"`

- Select multiple files with `Shift + Tab` and write to a file:

`find {{path/to/directory}} -type f | sk --multi > {{path/to/file}}`
