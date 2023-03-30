# homeshick 
## chatgpt 
The `homeshick` command is used to manage and organize dotfiles (hidden configuration files) in your home directory. 

Dotfiles are configuration files that start with a dot, such as `.bashrc`, `.vimrc`, and `.gitconfig`, and are used to store settings for different command line tools and applications. Managing and organizing these files can be a tedious task, especially when moving between different machines or operating systems.

Homeshick is a tool that provides a convenient way to manage dotfiles with Git. It tracks changes to dotfiles in a Git repository and allows you to easily synchronize those files across multiple machines.

The `homeshick` command provides various subcommands that allow you to interact with your dotfiles. Some common `homeshick` subcommands include:

- `homeshick clone`: Clones a Git repository containing your dotfiles.
- `homeshick link`: Creates symbolic links from your cloned dotfiles repository to your home directory.
- `homeshick pull`: Fetches changes from your dotfiles repository and updates your local files.
- `homeshick push`: Pushes changes to your dotfiles repository.
- `homeshick list`: Lists all the managed repositories.

Overall, `homeshick` is a powerful tool for organizing and maintaining your dotfiles, making it easy to switch between different machines and keep your configuration consistent. 

## tldr 
 
> Synchronize Git dotfiles.
> More information: <https://github.com/andsens/homeshick/wiki>.

- Create a new castle:

`homeshick generate {{castle_name}}`

- Add a file to your castle:

`homeshick track {{castle_name}} {{path/to/file}}`

- Go to a castle:

`homeshick cd {{castle_name}}`

- Clone a castle:

`homeshick clone {{github_username}}/{{repository_name}}`

- Symlink all files from a castle:

`homeshick link {{castle_name}}`
