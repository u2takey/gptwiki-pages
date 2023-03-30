# wajig 
## chatgpt 
The "wajig" command is a package management tool in Debian-based Linux distributions. It provides a user-friendly interface to perform various package management tasks such as searching, installing, removing, upgrading, and managing dependencies of the software packages.

Here are some of the most common commands used with wajig:

- "wajig sudo apt update": This command updates the package list and metadata from repositories.

- "wajig search <pkg_name>": This command searches for packages that match the specified package name.

- "wajig install <pkg_name>": This command installs the specified package and its dependencies.

- "wajig remove <pkg_name>": This command removes the specified package.

- "wajig purge <pkg_name>": This command removes the specified package and its configuration files.

- "wajig upgrade": This command upgrades all installed packages to their latest version.

- "wajig dist-upgrade": This command upgrades the distribution to the latest version.

- "wajig show <pkg_name>": This command displays detailed information about the specified package.

- "wajig list": This command lists all installed packages. 

Overall, the "wajig" command simplifies the management of software packages, making it easier for users to perform tasks efficiently. 

## tldr 
 
> Simplified all-in-one-place system support tool for Debian-based systems.
> More information: <https://wajig.togaware.com>.

- Update the list of available packages and versions:

`wajig update`

- Install a package, or update it to the latest available version:

`wajig install {{package}}`

- Remove a package and its configuration files:

`wajig purge {{package}}`

- Perform an update and then a dist-upgrade:

`wajig daily-upgrade`

- Display the sizes of installed packages:

`wajig sizes`

- List the version and distribution for all installed packages:

`wajig versions`

- List versions of upgradable packages:

`wajig toupgrade`

- Display packages which have some form of dependency on the given package:

`wajig dependents {{package}}`
