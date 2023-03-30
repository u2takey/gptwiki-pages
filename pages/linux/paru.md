# paru 
## chatgpt 
"paru" is a third-party package manager for Arch-based Linux distribution systems such as Arch Linux, Manjaro, and EndeavourOS. It is used to install, upgrade, and remove software packages from the system.

The command "paru" is used to invoke the package manager on the command line. It can be followed by various options and arguments to perform specific actions. For example, the command "paru -Syu" updates the system packages to their latest versions. Similarly, "paru -S package_name" installs the specified package on the system.

Here are some commonly used options and arguments with the "paru" command:

- "-S": Installs a package from the repositories
- "-Sy": Synchronizes the package databases with the servers
- "-Syu": Synchronizes the databases and updates all packages to their latest versions
- "-Syy": Refreshes the package database completely
- "-Ss": Searches for a package in the database
- "-Q": Lists all installed packages
- "-Qi package_name": Shows detailed information about an installed package
- "-Qu": Lists all available updates
- "-R package_name": Removes a package from the system

Overall, the "paru" command provides a streamlined way to manage packages on Arch-based Linux systems. 

## tldr 
 
> An AUR helper and pacman wrapper.
> More information: <https://github.com/Morganamilo/paru>.

- Interactively search for and install a package:

`paru {{package_name_or_search_term}}`

- Synchronize and update all packages:

`paru`

- Upgrade AUR packages:

`paru -Sua`

- Get information about a package:

`paru -Si {{package_name}}`

- Download `PKGBUILD` and other package source files from the AUR or ABS:

`paru --getpkgbuild {{package_name}}`

- Display the `PKGBUILD` file of a package:

`paru --getpkgbuild --print {{package_name}}`
