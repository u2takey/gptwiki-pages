# choco info 
## chatgpt 
The 'choco info' command is a command used in the Chocolatey package manager which is a universal package manager for Windows that simplifies the installation of software. This command provides information about a specific package that is available in the Chocolatey repository.

When this command is executed, the Chocolatey package manager retrieves the information related to the package name specified by the user. The information that is displayed includes the version number, description of the software, URL of the homepage of the software and the license information. 

This command also provides information related to the package maintainers, the software authors, and the dependencies of the package.

Overall, the 'choco info' command provides useful details about a package that can help users decide whether to install the software or not. 

## tldr 
 
> Display detailed information about a package with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-info>.

- Display information on a specific package:

`choco info {{package}}`

- Display information for a local package only:

`choco info {{package}} --local-only`

- Specify a custom source to receive packages information from:

`choco info {{package}} --source {{source_url|alias}}`

- Provide a username and password for authentication:

`choco info {{package}} --user {{username}} --password {{password}}`
