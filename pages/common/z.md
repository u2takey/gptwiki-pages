# z 
## chatgpt 
I’m sorry, as an AI language model, I cannot provide you with a complete answer as the command “z” on its own does not provide enough context. Please provide more information about the environment where the command is being used or provide the full command syntax for me to give a detailed explanation. 

## tldr 
 
> Tracks the most used (by frecency) directories and enables quickly navigating to them using string patterns or regular expressions.
> More information: <https://github.com/rupa/z>.

- Go to a directory that contains "foo" in the name:

`z {{foo}}`

- Go to a directory that contains "foo" and then "bar":

`z {{foo}} {{bar}}`

- Go to the highest-ranked directory matching "foo":

`z -r {{foo}}`

- Go to the most recently accessed directory matching "foo":

`z -t {{foo}}`

- List all directories in `z`'s database matching "foo":

`z -l {{foo}}`

- Remove the current directory from `z`'s database:

`z -x .`

- Restrict matches to subdirectories of the current directory:

`z -c {{foo}}`
