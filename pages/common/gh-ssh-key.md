# gh ssh-key 
## chatgpt 
The command "gh ssh-key" is a command line tool that allows users to manage their SSH keys with GitHub.

SSH (Secure Shell) keys are a secure way to authenticate your computer with a remote server. Using SSH keys allows you to log into a remote server securely without having to enter your password every time.

The "gh ssh-key" command can perform several functions such as creating a new SSH key, listing all SSH keys associated with your GitHub account, deleting an SSH key, or adding an SSH key to your GitHub account.

To use this command, you must have the GitHub CLI (Command Line Interface) installed on your computer. Once installed, you can run the "gh ssh-key" command in your terminal or command prompt, followed by the option that you want to use.

For example, to create a new SSH key, you can run the command "gh ssh-key create". This will prompt you to enter a name for your new key and where to save it on your computer. Once the key is created, you can add it to your GitHub account with the command "gh ssh-key add".

To list all SSH keys associated with your GitHub account, you can run the command "gh ssh-key list". This will display a list of all your SSH keys, their ID, and their name.

To delete an SSH key, you can run the command "gh ssh-key remove" followed by the ID of the key you want to delete.

Overall, the "gh ssh-key" command is a useful tool for managing your SSH keys with GitHub, allowing you to securely access remote servers and repositories. 

## tldr 
 
> Manage GitHub SSH keys from the command-line.
> More information: <https://cli.github.com/manual/gh_ssh-key>.

- Display help:

`gh ssh-key`

- List SSH keys for the currently authenticated user:

`gh ssh-key list`

- Add an SSH key to the currently authenticated user's account:

`gh ssh-key add {{path/to/key.pub}}`

- Add an SSH key to the currently authenticated user's account with a specific title:

`gh ssh-key add --title {{title}} {{path/to/key.pub}}`
