# choco pin 
## chatgpt 
The command "choco pin" is a command-line command for Chocolatey, a package manager for Windows. The primary function of the "choco pin" command is to 'pin' a package, which prevents it from being updated by Chocolatey.

When a package is pinned, Chocolatey will no longer attempt to update it to a newer version. This can be useful if you have a package that works with a specific version of software, and you don't want to risk breaking something by updating to a newer version.

The syntax of the "choco pin" command is as follows:

choco pin [options] <package names>

The "options" parameter is optional and can be used to further customize the "choco pin" command. Some of the different options available include specifying a version number to pin, unpinning a package, or listing currently pinned packages.

The "package names" parameter is required and refers to the name of the package you want to pin. You can specify one or more package names at once, separated by a space.

Overall, the "choco pin" command is a helpful tool for managing package updates and making sure your software remains at a version that works best for you. 

## tldr 
 
> Pin a package at a specific version with Chocolatey.
> Pinned packages are skipped automatically when upgrading.
> More information: <https://chocolatey.org/docs/commands-pin>.

- Display a list of pinned packages and their versions:

`choco pin list`

- Pin a package at its current version:

`choco pin add --name {{package}}`

- Pin a package at a specific version:

`choco pin add --name {{package}} --version {{version}}`

- Remove a pin for a specific package:

`choco pin remove --name {{package}}`
