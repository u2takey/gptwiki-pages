# scoop 
## chatgpt 
Scoop is a command-line package manager for Windows that automates the installation and uninstallation of software. Scoop simplifies the process of searching for and downloading software packages via the command line.

Here are some of the commonly used commands in Scoop:

- scoop install <package_name>: installs a package
- scoop uninstall <package_name>: uninstalls a package
- scoop list: displays the list of installed packages
- scoop update: updates all installed packages
- scoop search <keyword>: searches for a package using a keyword
- scoop status <package_name>: shows the status of a package.

Scoop can be used to install a wide range of open-source software packages, programming languages, and utilities. Scoop stores all installed packages in a central location, and can manage multiple software installations simultaneously.

Overall, Scoop is a useful tool for developers and system administrators who prefer to use the command line interface for software installation and management on Windows. 

## tldr 
 
> A command-line installer for Windows.
> More information: <https://scoop.sh>.

- Install a package:

`scoop install {{package}}`

- Remove a package:

`scoop uninstall {{package}}`

- Update all installed packages:

`scoop update --all`

- List installed packages:

`scoop list`

- Display information about a package:

`scoop info {{package}}`

- Search for a package:

`scoop search {{package}}`

- Remove old versions of all packages and clear the download cache:

`scoop cleanup --cache --all`
