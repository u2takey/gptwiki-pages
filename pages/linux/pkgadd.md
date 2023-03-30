# pkgadd 
## chatgpt 
The `pkgadd` command is a utility command used in Solaris and other Unix-based operating systems to install software packages from a distribution medium such as a CD-ROM. 

The command typically needs to be executed as a superuser or with the `su` command to override user restrictions. 

When run, `pkgadd` prompts the user for various options and information, such as which package to install, where to install it, and which dependencies to include. It then proceeds to unpack and install the selected package and its associated files, registering it with the system's package management system.

Overall, `pkgadd` simplifies the installation process for software packages and helps to ensure that all dependencies are correctly installed and configured, making it an essential tool for systems administrators and developers. 

## tldr 
 
> Add a package to a CRUX system.
> More information: <https://docs.oracle.com/cd/E19253-01/816-5166/pkgadd-1m/index.html>.

- Install a local software package:

`pkgadd {{package_name}}`

- Update an already installed package from a local package:

`pkgadd -u {{package_name}}`
