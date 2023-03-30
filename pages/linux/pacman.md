# pacman 
## chatgpt 
Pacman is a package manager utility used in Arch Linux and its derivatives for managing software packages. It is used to install, remove, update, and search for packages. 

Here are some common commands used with Pacman: 

1. `pacman -S package_name`: Installs the specified package. For example, `pacman -S firefox` installs the Firefox web browser.

2. `pacman -Ss search_term`: Searches for packages that match the specified search term. For example, `pacman -Ss text editor` would return a list of text editors available in the package repository.

3. `pacman -Syu`: Updates all installed packages. The -Sy option updates the package lists while -u actually updates the packages.

4. `pacman -R package_name`: Removes the specified package. For example, `pacman -R firefox` would remove the Firefox web browser.

5. `pacman -Q`: Lists all installed packages.

6. `pacman -Sw package_name`: Downloads the specified package without installing it.

7. `pacman -Qi package_name`: Shows information about the specified package, including version, description, and dependencies.

8. `pacman -Sc`: Deletes old versions of packages from the package cache.

In addition to these basic commands, Pacman supports many other options and features for managing software packages on a Linux system. 

## tldr 
 
> Arch Linux package manager utility.
> Some subcommands such as `pacman sync` have their own usage documentation.
> For equivalent commands in other package managers, see <https://wiki.archlinux.org/title/Pacman/Rosetta>.
> More information: <https://man.archlinux.org/man/pacman.8>.

- Synchronize and update all packages:

`sudo pacman -Syu`

- Install a new package:

`sudo pacman -S {{package_name}}`

- Remove a package and its dependencies:

`sudo pacman -Rs {{package_name}}`

- Search the package database for a regular expression or keyword:

`pacman -Ss "{{search_pattern}}"`

- List installed packages and versions:

`pacman -Q`

- List only the explicitly installed packages and versions:

`pacman -Qe`

- List orphan packages (installed as dependencies but not actually required by any package):

`pacman -Qtdq`

- Empty the entire pacman cache:

`sudo pacman -Scc`
