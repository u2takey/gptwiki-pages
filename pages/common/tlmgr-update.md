# tlmgr update 
## chatgpt 
The command "tlmgr update" is used in the TeX Live distribution to update all installed packages to their latest version.

When executed, the command initiates the TeX Live package manager (tlmgr) and checks for updates to all installed packages. If any updates are available, tlmgr downloads and installs them automatically.

It is recommended to run this command periodically to keep all TeX packages up-to-date and ensure that your TeX distribution has the latest bug fixes and features. 

Note: To use this command, you need to have administrative privileges on your system. 

## tldr 
 
> Update TeX Live packages.
> More information: <https://www.tug.org/texlive/tlmgr.html>.

- Update all TeX Live packages:

`sudo tlmgr update --all`

- Update tlmgr itself:

`sudo tlmgr update --self`

- Update a specific package:

`sudo tlmgr update {{package}}`

- Update all except a specific package:

`sudo tlmgr update --all --exclude {{package}}`

- Update all packages, making a backup of the current packages:

`sudo tlmgr update --all --backup`

- Update a specific package without updating its dependencies:

`sudo tlmgr update --no-depends {{package}}`

- Simulate updating all packages without making any changes:

`sudo tlmgr update --all --dry-run`
