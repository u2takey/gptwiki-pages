# choco outdated 
## chatgpt 
The "choco outdated" command is used in Chocolatey, a package manager for Windows, to check for outdated packages that have been previously installed using Chocolatey. 

When this command is executed, Chocolatey performs a scan of installed packages and compares their versions with the versions currently available on its official repository. If a newer version of a package is found, Chocolatey lists it as an outdated package.

This command is useful because it allows you to quickly identify which packages are outdated and are in need of an update. It saves you from having to manually check each package individually for updates. 

However, it's important to note that the "choco outdated" command only checks for outdated packages that were installed using Chocolatey. It does not list packages installed through other means. 

## tldr 
 
> Check for outdated packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-outdated>.

- Display a list of outdated packages in table format:

`choco outdated`

- Ignore pinned packages in the output:

`choco outdated --ignore-pinned`

- Specify a custom source to check packages from:

`choco outdated --source {{source_url|alias}}`

- Provide a username and password for authentication:

`choco outdated --user {{username}} --password {{password}}`
