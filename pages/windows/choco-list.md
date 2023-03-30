# choco list 
## chatgpt 
The command "choco list" is a Chocolatey command-line command that lists the currently installed and available packages in the Chocolatey package repository.

Detailed explanation:

Chocolatey is a package manager for Windows that helps to automate software installation, upgrades, and uninstallation. It works by downloading packages from a centralized repository which contains a large number of software packages. 

The "choco list" command is used to list the currently installed and available packages in the Chocolatey package repository. 

When executed, the command will display a list of all packages that are currently installed on your computer. Additionally, it will also display all available packages that can be installed using Chocolatey.

The result of the "choco list" command is displayed in the console window in alphabetical order. The output will include the package name, version number, and a brief description of each package.

Overall, the "choco list" command is a useful one to get a quick overview of the packages installed on your computer or to search for new packages that you may want to install. 

## tldr 
 
> Display a list of packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-list>.

- Display all available packages:

`choco list`

- Display all locally installed packages:

`choco list --local-only`

- Display a list including local programs:

`choco list --include-programs`

- Display only approved packages:

`choco list --approved-only`

- Specify a custom source to display packages from:

`choco list --source {{source_url|alias}}`

- Provide a username and password for authentication:

`choco list --user {{username}} --password {{password}}`
