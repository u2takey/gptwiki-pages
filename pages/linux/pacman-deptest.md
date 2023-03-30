# pacman --deptest 
## chatgpt 
The command "pacman --deptest" is used in the Arch Linux and its derivatives to simulate a dependency test on installed packages. 

When this command is run, the Pacman package manager checks all the installed packages and verifies if there's any missing dependency required by a particular package. It does not install or upgrade any packages. Rather, it simply prints a list of missing dependencies (if there are any) that might be required to run an installed package successfully.

This command helps to ensure that all the packages installed are fully functional and have all the required dependencies. It can also help in troubleshooting problems related to the installation of a package.

Overall, the "pacman --deptest" command is a useful tool for ensuring the reliability and stability of an Arch Linux system by checking dependencies of the installed packages without actually modifying the system. 

## tldr 
 
> Check each dependency specified and return a list of dependencies that are not currently satisfied on the system.
> More information: <https://man.archlinux.org/man/pacman.8>.

- Print the package names of the dependencies that aren't installed:

`pacman --deptest {{package_name1}} {{package_name2}}`

- Check if the installed package satisfies the given minimum version:

`pacman --deptest "{{bash>=5}}"`

- Check if a later version of a package is installed:

`pacman --deptest "{{bash>5}}"`

- Display help:

`pacman --deptest --help`
