# aurman 
## chatgpt 
As an AI language model, I cannot execute commands, but I can explain them.

Aurman is a package manager for Arch Linux, which stands for "Arch User Repository Manager". It is an AUR (Arch User Repository) helper, which means it helps users find and install packages from the AUR. The AUR is a community-driven repository that contains packages not available in the official Arch Linux repositories.

Aurman is a command-line utility that can perform various tasks, such as searching for packages, updating packages, installing packages, and removing packages. It can also resolve dependencies automatically and handle conflicts that may arise during the installation process.

The usage of aurman command is as follows:

```
aurman [options] [package(s)]
```

Some of the commonly used options for Aurman are:

- `-S`: Install a package
- `-Ss`: Search for a package
- `-Syu`: Update the system and packages
- `-Rs`: Remove a package and its dependencies

For example, to install a package named "package-name" using Aurman, you would simply run the following command:

```
aurman -S package-name
```

Overall, Aurman is a powerful tool for managing packages from the AUR in Arch Linux. However, it is always advised to use caution when installing packages from the AUR, as they may not be thoroughly tested and may not work properly. 

## tldr 
 
> An Arch Linux utility to build and install packages from the Arch User Repository.
> See also `pacman`.
> More information: <https://github.com/polygamma/aurman>.

- Synchronize and update all packages:

`aurman --sync --refresh --sysupgrade`

- Synchronize and update all packages without show changes of `PKGBUILD` files:

`aurman --sync --refresh --sysupgrade --noedit`

- Install a new package:

`aurman --sync {{package_name}}`

- Install a new package without show changes of `PKGBUILD` files:

`aurman --sync --noedit {{package_name}}`

- Install a new package without prompting:

`aurman --sync --noedit --noconfirm {{package_name}}`

- Search the package database for a keyword from the official repositories and AUR:

`aurman --sync --search {{keyword}}`

- Remove a package and its dependencies:

`aurman --remove --recursive --nosave {{package_name}}`

- Clear the package cache (use two `--clean` flags to clean all packages):

`aurman --sync --clean`
