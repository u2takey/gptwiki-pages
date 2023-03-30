# slapt-get 
## chatgpt 
Slapt-get is a command-line tool for managing packages on Slackware-based Linux distributions. It is the equivalent of the apt-get or yum commands on other Linux distributions.

The slapt-get command retrieves, updates, installs, and removes packages from the official Slackware package repositories or from third-party repositories. It can also resolve dependencies automatically and install missing packages.

Here are some common usages of slapt-get:

1. Update package list:
To update the package list, run the following command:

`slapt-get --update`

This command will download the latest package information from the repository.

2. Upgrade packages:
To upgrade all installed packages to their latest version, run the following command:

`slapt-get --upgrade`

This command will download and install the latest versions of all installed packages.

3. Install a package:
To install a package, run the following command:

`slapt-get --install <packagename>`

Replace <packagename> with the name of the package you want to install.

4. Remove a package
To remove a package, run the following command:

`slapt-get --remove <packagename>`

Replace <packagename> with the name of the package you want to remove.

5. Search for a package:
To search for a specific package, run the following command:

`slapt-get --search <packagename>`

Replace <packagename> with the name of the package you want to search for.

These are just some of the common usages of the slapt-get command. It is a powerful tool that can be used to manage packages on Slackware-based Linux distributions. 

## tldr 
 
> An apt like system for Slackware package management.
> Package sources need to be configured in the slapt-getrc file.
> More information: <https://software.jaos.org>.

- Update the list of available packages and versions:

`slapt-get --update`

- Install a package, or update it to the latest available version:

`slapt-get --install {{package_name}}`

- Remove a package:

`slapt-get --remove {{package_name}}`

- Upgrade all installed packages to their latest available versions:

`slapt-get --upgrade`

- Locate packages by the package name, disk set, or version:

`slapt-get --search {{package_name}}`

- Show information about a package:

`slapt-get --show {{package_name}}`
