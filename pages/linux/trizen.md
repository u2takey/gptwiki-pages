# trizen 
## chatgpt 
Trizen is a command-line package manager for Arch-based Linux distributions. With Trizen, users can easily search, install, and manage software packages from the Arch User Repository (AUR) as well as the standard Arch Linux repositories.

Here are some commonly used Trizen commands:

1. trizen -S packagename - Install a package from the Arch repositories.
2. trizen -Syu - Update system and packages.
3. trizen -Ss keyword - Search for a package by keyword.
4. trizen -Syy - Refresh package database.
5. trizen -Rs packagename - Remove a package.
6. trizen -Qe - List all packages installed through Trizen.
7. trizen -Qo /path/to/file - Determine which package a file belongs to.
8. trizen -Si packagename - Display information about a package.

Overall, Trizen makes it easy for Arch Linux users to find and manage software packages, both from the official repositories and from the community-maintained AUR. 

## tldr 
 
> Arch Linux utility for building packages from the Arch User Repository (AUR).
> More information: <https://github.com/trizen/trizen>.

- Synchronize and update all AUR packages:

`trizen -Syua`

- Install a new package:

`trizen -S {{package}}`

- Remove a package and its dependencies:

`trizen -Rs {{package}}`

- Search the package database for a keyword:

`trizen -Ss {{keyword}}`

- Show information about a package:

`trizen -Si {{package}}`

- List installed packages and versions:

`trizen -Qe`
