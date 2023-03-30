# dpkg 
## chatgpt 
The "dpkg" command refers to the Debian Package Manager, a tool for managing installed software packages on Debian-based operating systems. 

The dpkg command is used to install, remove, and manage packages, as well as querying the current package status and dependencies.

Some common use cases of dpkg include:

- Installing a package: `sudo dpkg -i package.deb` (This command will install the package with the given filename)
- Removing a package: `sudo dpkg -r package-name` (This command will remove the package with the given name)
- Checking if a package is installed: `dpkg -s package-name` (This command will show information about the package with the given name)
- Listing all installed packages: `dpkg -l` (This command will list all packages installed on the system)

It is important to note that dpkg is a low-level tool and should be used with caution, as it does not handle dependencies automatically. To properly manage dependencies, it is recommended to use a higher-level tool such as apt or apt-get. 

## tldr 
 
> Debian package manager.
> Some subcommands such as `dpkg deb` have their own usage documentation.
> For equivalent commands in other package managers, see <https://wiki.archlinux.org/title/Pacman/Rosetta>.
> More information: <https://manpages.debian.org/latest/dpkg/dpkg.html>.

- Install a package:

`dpkg -i {{path/to/file.deb}}`

- Remove a package:

`dpkg -r {{package_name}}`

- List installed packages:

`dpkg -l {{pattern}}`

- List a package's contents:

`dpkg -L {{package_name}}`

- List contents of a local package file:

`dpkg -c {{path/to/file.deb}}`

- Find out which package owns a file:

`dpkg -S {{filename}}`
