# apt-mark 
## chatgpt 
apt-mark is a command used in Linux-based operating systems, such as Ubuntu, Debian, and others, to manipulate the system's package marking database. 

The package marking database tracks the state of packages on the system, such as whether they are installed, hold, or auto-installed. apt-mark is used to interact with this database, and the following are some of the ways it can be used:

1. To hold a package: Using the command "apt-mark hold <package-name>", users can mark a package as held back from updates. This ensures that even if an update is available for the package, it will not be installed automatically unless the hold is removed.

2. To unhold a package: Users can use "apt-mark unhold <package-name>" to remove the hold on a package, allowing it to be updated.

3. To mark a package as auto-installed: Users can use "apt-mark auto <package-name>" to mark a package as auto-installed, which means that if no other package depends on it, it will be automatically removed from the system during package cleanup.

4. To mark a package as manual: If a package was auto-installed but the user wants to keep it, they can use "apt-mark manual <package-name>" to mark it as a manual package.

5. To show package status: Using "apt-mark showmanual" or "apt-mark showauto", users can view the list of packages that are manual and auto-installed, respectively.

Overall, apt-mark is a useful tool for managing package dependencies and controlling the state of packages on the system. 

## tldr 
 
> Utility to change the status of installed packages.
> More information: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

- Mark a package as automatically installed:

`sudo apt-mark auto {{package_name}}`

- Hold a package at its current version and prevent updates to it:

`sudo apt-mark hold {{package_name}}`

- Allow a package to be updated again:

`sudo apt-mark unhold {{package_name}}`

- Show manually installed packages:

`apt-mark showmanual`

- Show held packages that aren't being updated:

`apt-mark showhold`
