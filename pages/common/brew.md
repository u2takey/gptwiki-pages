# brew 
## chatgpt 
Brew is a package manager for macOS that allows users to easily install and manage various Unix tools, libraries, and other software packages from the command line.

When you run the `brew` command in the Terminal, it will display a list of available subcommands and options that you can use to manage your installed packages. Some of the commonly used subcommands include:

- `brew install [package]`: This command allows you to download and install a specific package from the official Homebrew repository. For example, `brew install python` will install the Python programming language on your machine.

- `brew upgrade`: This command will check for updated packages and upgrade any outdated packages to their latest versions.

- `brew list`: This command lists all the currently installed packages on your machine.

- `brew cask`: This subcommand allows you to install macOS applications and manage them similarly to other brew packages.

Overall, `brew` simplifies the process of installing and managing various programs and tools on your macOS system. 

## tldr 
 
> Package manager for macOS and Linux.
> More information: <https://brew.sh>.

- Install the latest stable version of a formula or cask (use `--devel` for development versions):

`brew install {{formula}}`

- List all installed formulae and casks:

`brew list`

- Upgrade an installed formula or cask (if none is given, all installed formulae/casks are upgraded):

`brew upgrade {{formula}}`

- Fetch the newest version of Homebrew and of all formulae and casks from the Homebrew source repository:

`brew update`

- Show formulae and casks that have a more recent version available:

`brew outdated`

- Search for available formulae (i.e. packages) and casks (i.e. native packages):

`brew search {{text}}`

- Display information about a formula or a cask (version, installation path, dependencies, etc.):

`brew info {{formula}}`

- Check the local Homebrew installation for potential problems:

`brew doctor`
