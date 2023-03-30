# fish 
## chatgpt 
The "fish" command is a shell command used to launch the Fish shell, which is a simple, user-friendly and interactive shell for the UNIX-like operating systems. 

When you type "fish" in the terminal and hit enter, the Fish shell will be launched, and you will immediately see a new command prompt with the Fish shell's default prompt.

Fish shell offers several features such as syntax highlighting, easy-to-use tab completions, and a powerful scripting language.

Using the Fish shell, you can run all the standard UNIX commands, including ls, cd, and mkdir, and you can also customize the prompt, add aliases, and customize the shell environment variables.

Overall, the "fish" command is used as a shortcut to launch the Fish shell and work on the terminal in a more interactive and user-friendly manner. 

## tldr 
 
> The Friendly Interactive SHell, a command-line interpreter designed to be user friendly.
> More information: <https://fishshell.com>.

- Start an interactive shell session:

`fish`

- Start an interactive shell session without loading startup configs:

`fish --no-config`

- Execute specific commands:

`fish --command "{{echo 'fish is executed'}}"`

- Execute a specific script:

`fish {{path/to/script.fish}}`

- Check a specific script for syntax errors:

`fish --no-execute {{path/to/script.fish}}`

- Execute specific commands from `stdin`:

`{{echo "echo 'fish is executed'"}} | fish`

- Start an interactive shell session in private mode, where the shell does not access old history or save new history:

`fish --private`

- Define and export an environmental variable that persists across shell restarts (builtin):

`set --universal --export {{variable_name}} {{variable_value}}`
