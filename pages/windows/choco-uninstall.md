# choco uninstall 
## chatgpt 
"choco uninstall" is a command used with Chocolatey, a command-line package manager for Windows, to uninstall a package previously installed using Chocolatey. 

Syntax: choco uninstall [packageName] [options]

[packageName] is the name of the package to be uninstalled.

[options] are additional settings and customization for the uninstall process such as, specifying the version to uninstall, forcing the uninstallation without confirmation, etc. 

Examples:
choco uninstall googlechrome: Uninstalls the Google Chrome package.
choco uninstall git --version 2.30.2: Uninstalls Git version 2.30.2 using Chocolatey.
choco uninstall notepadplusplus --force: Uninstalls Notepad++ without confirmation. 

Note: This command only uninstalls packages installed using Chocolatey. To remove a program installed through other means, you need to use the appropriate uninstaller or through the Windows Control Panel. 

## tldr 
 
> Uninstall one or more packages with Chocolatey.
> More information: <https://chocolatey.org/docs/commands-uninstall>.

- Uninstall one or more space-separated packages:

`choco uninstall {{package1 package2 ...}}`

- Uninstall a specific version of a package:

`choco uninstall {{package}} --version {{version}}`

- Confirm all prompts automatically:

`choco uninstall {{package}} --yes`

- Remove all dependencies when uninstalling:

`choco uninstall {{package}} --remove-dependencies`

- Uninstall all packages:

`choco uninstall all`
