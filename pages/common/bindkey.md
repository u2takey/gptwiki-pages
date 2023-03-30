# bindkey 
## chatgpt 
The `bindkey` command is a Unix shell command that is used to assign actions or functions to specific keys or key combinations on the keyboard. When you run the `bindkey` command, you can bind various functions or actions to the specified key or key combination. 

Here's an example: let's say you want to bind the `Ctrl + X` key combination to the "cut" command in your terminal. First, you would type `bindkey -e` to put the terminal in "emacs mode". Then, you would run the command `bindkey "^X" backward-kill-word` to bind the `Ctrl + X` key combination to the "backward-kill-word" function, which deletes the word behind the cursor. 

There are many other possible uses for the `bindkey` command, such as binding keys to enter specific strings, executing scripts or functions, navigating directories, and more. Overall, `bindkey` is a useful command for customizing your shell environment and making it more efficient for your personal workflow. 

## tldr 
 
> Add keybindings to Z-Shell.
> More information: <https://zsh.sourceforge.io/Guide/zshguide04.html>.

- Bind a hotkey to a specific command:

`bindkey "{{^k}}" {{kill-line}}`

- Bind a hotkey to a specific key sequence:

`bindkey -s '^o' 'cd ..\n'`

- View keymaps:

`bindkey -l`

- View the hotkey in a keymap:

`bindkey -M main`
