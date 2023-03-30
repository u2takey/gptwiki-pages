# apt-get 
## chatgpt 
apt-get is a command line tool used in the Debian and Ubuntu operating systems for package management. It helps in installing, removing, and updating software packages. 

Here’s a brief overview of the most common uses of the apt-get command:

1. Update package index: 
      apt-get update command downloads the package information from all configured sources and updates the local package database on your system. 

2. Install a package:
      The syntax for installing a package using the apt-get command is: 
      apt-get install package_name
      This command installs the specified package along with all its dependencies. 

3. Remove a package:
      The syntax for removing a package using the apt-get command is:
      apt-get remove package_name
      This command removes the specified package from your system. 

4. Upgrade system packages:
      The syntax for upgrading your system packages using the apt-get command is:
      apt-get upgrade
      This command upgrades all the installed packages to their latest version. 

5. Search for a package:
      The syntax for searching for a package using the apt-get command is:
      apt-get search package_name
      This command lists out all the packages that match the specified keyword. 

6. Clear cache:
      The syntax for clearing the apt cache using the apt-get command is:
      apt-get clean
      This command clears out the package cache on your system. 

These are some of the most common uses of the apt-get command. It is an important tool for package management in Debian and Ubuntu based systems. 

## tldr 
 
> Debian and Ubuntu package management utility.
> Search for packages using `apt-cache`.
> More information: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

- Update the list of available packages and versions (it's recommended to run this before other `apt-get` commands):

`apt-get update`

- Install a package, or update it to the latest available version:

`apt-get install {{package}}`

- Remove a package:

`apt-get remove {{package}}`

- Remove a package and its configuration files:

`apt-get purge {{package}}`

- Upgrade all installed packages to their newest available versions:

`apt-get upgrade`

- Clean the local repository - removing package files (`.deb`) from interrupted downloads that can no longer be downloaded:

`apt-get autoclean`

- Remove all packages that are no longer needed:

`apt-get autoremove`

- Upgrade installed packages (like `upgrade`), but remove obsolete packages and install additional packages to meet new dependencies:

`apt-get dist-upgrade`
