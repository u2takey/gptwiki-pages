# xbps 
## chatgpt 
xbps is a command-line package manager for the XBPS package format used by Void Linux. It allows users to search and install software packages, remove installed packages, update the system and manage repositories.

Here are the most common options used with the xbps command:

- `xbps-query`: Used to search for available packages in the repositories.
- `xbps-install`: Used to install packages from the repositories.
- `xbps-remove`: Used to remove installed packages.
- `xbps-upgrade`: Used to update the system to the latest version of all installed packages.

The command can also be used with additional options for customized package installation or package querying. For example, `xbps-install -Su` can be used to update the system and upgrade all installed packages to their latest version. 

Overall, xbps is a powerful tool that allows users to manage packages and updates on Void Linux systems through the command-line interface. 

## tldr 
 
> The X Binary Package System (or xbps) is the binary package system used by Void Linux.
> More information: <https://github.com/void-linux/xbps>.

- Install packages and synchronize them with the remote repository:

`xbps-install --sync {{package_name1}} {{package_name2}}`

- Search for a package in the remote repository:

`xbps-query --repository -s {{package_name}}`

- Remove a package, leaving all of its dependencies installed:

`xbps-remove {{package_name}}`

- Remove a package and all of its dependencies recursively that are not required by other packages:

`xbps-remove --recursive {{package_name}}`

- Synchronize your repository databases and update your system and dependencies:

`xbps-install --sync --update`

- Remove packages that were installed as dependencies and aren't currently needed:

`xbps-remove --remove-orphans`

- Remove obsolete packages from the cache:

`xbps-remove --clean-cache`
