# synopkg 
## chatgpt 
The "synopkg" command is a package manager tool used in Synology DiskStation devices. It allows users to install, manage, and remove various software packages and extensions on their Synology NAS. 

The commands and options available in synopkg vary depending on the version of DSM installed and the packages installed on the device. Some common commands include:

 - `synopkg install <package>`: This command installs a package by specifying the name of the package to be installed.

- `synopkg remove <package>`: This command removes a package by specifying the name of the package to be removed.

- `synopkg update`: This command updates all installed packages and their dependencies.

- `synopkg search <keyword>`: This command lists all available packages that match the keyword specified.

- `synopkg list`: This command lists all the installed packages along with their status.

- `synopkg start <package>`: This command starts a stopped package.

- `synopkg stop <package>`: This command stops a running package.

Overall, synopkg provides Synology users with a simple way to manage and maintain software packages on their DiskStation devices. 

## tldr 
 
> Package management utility for Synology DiskStation Manager.
> More information: <https://www.synology.com/dsm>.

- List the names of installed packages:

`synopkg list --name`

- List packages which depend on a specific package:

`synopkg list --depend-on {{package}}`

- Start/Stop a package:

`sudo synopkg {{start|stop}} {{package}}`

- Print the status of a package:

`synopkg status {{package}}`

- Uninstall a package:

`sudo synopkg uninstall {{package}}`

- Check if updates are available for a package:

`synopkg checkupdate {{package}}`

- Upgrade all packages to the latest version:

`sudo synopkg upgradeall`

- Install a package from a synopkg file:

`sudo synopkg install {{path/to/package.spk}}`
