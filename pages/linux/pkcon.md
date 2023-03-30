# pkcon 
## chatgpt 
The "pkcon" command is a Linux package management tool for managing software packages. "pkcon" stands for "PackageKit Console Client", which means it is a console-based interface for interacting with the system's package manager.

With "pkcon", you can perform various actions related to package management, such as searching for new packages, installing, upgrading, or removing existing packages, and maintaining the system's package repository.

Some examples of "pkcon" commands include:

- "pkcon search": This command allows you to search for specific packages or keywords related to packages.
- "pkcon install": This command installs a package onto the system. You can specify the package name or a package file location to install.
- "pkcon update": This command updates all the installed packages on the system to their latest version available in the repository.
- "pkcon remove": This command removes an installed package from the system.

"pkcon" is a useful tool for managing packages on Linux systems, especially for those who prefer a command-line interface. It can be used on various Linux distributions that use PackageKit as their package management system, such as Fedora, Debian, and Ubuntu. 

## tldr 
 
> Command line client for PackageKit console program used by Discover and Gnome software and alternative to 'apt'.
> More information: <https://manned.org/pkcon>.

- Install a package:

`pkcon install {{package}}`

- Remove a package:

`pkcon remove {{package}}`

- Refresh the package cache:

`pkcon refresh`

- Update packages:

`pkcon update`

- Search for a specific package:

`pkcon search {{package}}`

- List all available packages:

`pkcon get-packages`
