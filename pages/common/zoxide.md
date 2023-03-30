# zoxide 
## chatgpt 
Zoxide is a command-line tool for fast directory navigation. It keeps track of the directories you use frequently and learns which ones you use most often. When you type a directory path, zoxide suggests which directories you are most likely to be looking for, based on your usage history. This saves time and keystrokes when navigating your file system.

To use zoxide, you need to install it first. Installation instructions can be found on its official website.

Once installed, you can use the following commands:

- "z" - Displays the directory list and their corresponding scores. You can navigate to any directory on the list by typing its score number.

- "z <directory>" - Finds the best matching directory based on your usage history and jumps directly to that directory.

- "z -c" - Clears the history of your file system usage.

- "z -h" - Displays help information about the command.

- "z -i" - Returns information on how to integrate zoxide with your shell.

- "z -l" - Displays a list of all directories currently tracked by zoxide, sorted by usage frequency.

- "z -r" - Removes a directory from the history of your file system usage.

Overall, zoxide is a powerful tool that can help to save a lot of time when navigating the file system, especially if you use the command line frequently. 

## tldr 
 
> Keep track of the most frequently used directories.
> Uses a ranking algorithm to navigate to the best match.
> More information: <https://github.com/ajeetdsouza/zoxide>.

- Go to the highest-ranked directory that contains "foo" in the name:

`zoxide query {{foo}}`

- Go to the highest-ranked directory that contains "foo" and then "bar":

`zoxide query {{foo}} {{bar}}`

- Start an interactive directory search (requires `fzf`):

`zoxide query --interactive`

- Add a directory or increment its rank:

`zoxide add {{path/to/directory}}`

- Remove a directory from `zoxide`'s database interactively:

`zoxide remove {{path/to/directory}} --interactive`

- Generate shell configuration for command aliases (`z`, `za`, `zi`, `zq`, `zr`):

`zoxide init {{bash|fish|zsh}}`
