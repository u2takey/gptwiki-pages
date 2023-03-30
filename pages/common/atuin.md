# atuin 
## chatgpt 
I'm sorry but "atuin" does not appear to be a valid command in any commonly-used operating system, programming language, or software application. Can you please provide more context or information about where you encountered this command and in what context it was used? 

## tldr 
 
> Store your shell history in a searchable database.
> Optionally sync your encrypted history between machines.
> More information: <https://atuin.sh/docs/overview/introduction/>.

- Install atuin into your shell:

`eval "$(atuin init {{bash|zsh|fish}})"`

- Import history from the shell default history file:

`atuin import auto`

- Search shell history for a specific command:

`atuin search {{command}}`

- Register an account on the default sync server:

`atuin register -u {{username}} -e {{email}} -p {{password}}`

- Login to the default sync server:

`atuin login -u {{username}} -p {{password}}`

- Sync history with the sync server:

`atuin sync`
