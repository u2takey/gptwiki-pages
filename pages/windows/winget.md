# winget 
## chatgpt 
The "winget" command is used to interact with the Windows Package Manager, which is a new package manager for Windows. The Windows Package Manager allows users to easily download and install software packages from a command-line interface.

When the "winget" command is entered into the command prompt, it will display a list of available commands and options that can be used with the Windows Package Manager. Some of the common commands include:

- install: Used to install packages from the Windows Package Manager repository
- search: Used to find packages in the repository based on a search string
- show: Used to display information about a specific package
- list: Used to display a list of installed packages
- upgrade: Used to upgrade packages to the latest version

To use the "winget" command, open the command prompt and type "winget" followed by the desired command and any necessary parameters. For example, to install a package named "Visual Studio Code", you would enter the following command:

winget install "Visual Studio Code"

The Windows Package Manager will then download and install the software package automatically, without requiring any user intervention. This can be useful for system administrators or users who need to quickly install multiple software packages on a Windows machine. 

## tldr 
 
> Windows Package Manager CLI.
> More information: <https://learn.microsoft.com/windows/package-manager/winget>.

- Install a package:

`winget install {{package}}`

- Display information about a package:

`winget show {{package}}`

- Search for a package:

`winget search {{package}}`

- Upgrade all packages to latest versions:

`winget upgrade --all`

- List all packages installed that can be managed with winget:

`winget list --source winget`
