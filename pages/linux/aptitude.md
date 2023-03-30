# aptitude 
## chatgpt 
"aptitude" is a command-line package management tool for Debian-based Linux systems, such as Ubuntu. It allows users to search, manage, and install software packages from the command line.

Some of the key functions of the "aptitude" command include the following:

1. Updating package lists: The "aptitude update" command refreshes the local package database, ensuring that any available updates or new packages are included.

2. Searching for packages: The "aptitude search" command allows users to search for specific packages by name, description, or keyword.

3. Installing packages: The "aptitude install" command installs new packages onto the system. Users can specify a single package or a list of packages to install.

4. Removing packages: The "aptitude remove" command uninstalls packages from the system. Users can specify a single package or a list of packages to remove.

5. Upgrading packages: The "aptitude upgrade" command upgrades all installed packages to their latest versions. 

6. Displaying package information: The "aptitude show" command displays detailed information about a specific package, including its description, version, dependencies, and installation status.

Overall, "aptitude" is a powerful tool for managing software packages on Debian-based Linux systems. It offers a variety of options and commands for finding, installing, and removing packages, as well as keeping the system up-to-date with the latest versions. 

## tldr 
 
> Debian and Ubuntu package management utility.
> More information: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

- Synchronize list of packages and versions available. This should be run first, before running subsequent aptitude commands:

`aptitude update`

- Install a new package and its dependencies:

`aptitude install {{package}}`

- Search for a package:

`aptitude search {{package}}`

- Search for an installed package (`?installed` is an aptitude search term):

`aptitude search '?installed({{package}})'`

- Remove a package and all packages depending on it:

`aptitude remove {{package}}`

- Upgrade installed packages to the newest available versions:

`aptitude upgrade`

- Upgrade installed packages (like `aptitude upgrade`) including removing obsolete packages and installing additional packages to meet new package dependencies:

`aptitude full-upgrade`

- Put an installed package on hold to prevent it from being automatically upgraded:

`aptitude hold '?installed({{package}})'`
