# pacman --query 
## chatgpt 
The command "pacman --query" is used to query the package database of the Pacman package manager in Arch Linux. This command is used to search for information on installed or available packages.

When executed, the "pacman --query" command displays a list of all installed packages in the system along with their version numbers and installation date. It also shows the dependencies for each package, which are the other packages required for the installed package to function properly.

Additionally, the "pacman --query" command can be used with various options such as:

- "-Qe" to list all explicitly installed packages
- "-Ql" to list all installed files for a given package
- "-Qi" to display detailed information on a specific package
- "-Ss" to search for packages in the database that match a given string

Overall, the "pacman --query" command is a useful tool for managing packages and dependencies in an Arch Linux system. 

## tldr 
 
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

- List installed packages and versions:

`pacman --query`

- List only packages and versions that were explicitly installed:

`pacman --query --explicit`

- Find which package owns a file:

`pacman --query --owns {{filename}}`

- Display information about an installed package:

`pacman --query --info {{package_name}}`

- List files owned by a package:

`pacman --query --list {{package_name}}`

- List orphan packages (installed as dependencies but not required by any package):

`pacman --query --unrequired --deps --quiet`

- List installed packages not found in the repositories:

`pacman --query --foreign`

- List outdated packages:

`pacman --query --upgrades`
