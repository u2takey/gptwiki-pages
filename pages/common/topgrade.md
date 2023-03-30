# topgrade 
## chatgpt 
The "topgrade" command refers to a tool that can be used on Unix or Linux systems to update all installed packages and software to their latest versions.

When executed, the "topgrade" command will scan the system to determine which packages are installed and which upgrades are available. It will then proceed to download and install the latest version of each package, along with any necessary dependencies.

The "topgrade" command offers several benefits, including:

1. Automated updates: "topgrade" automates the update process, which saves time and effort that would otherwise have been spent manually updating each package.

2. Security updates: The tool checks for security patches for installed software and installs them with the update.

3. Conflict resolution: The tool automatically detects conflicts and offers solutions to fix them.

4. Customization: The user can configure the tool to exclude certain packages or select a specific update interval according to their preferences.

Overall, the "topgrade" command is a useful tool for system administrators or anyone looking to keep their Unix or Linux system updated and secure. 

## tldr 
 
> Update all applications on the system.
> More information: <https://github.com/r-darwish/topgrade>.

- Run updates:

`topgrade`

- Say yes to all updates:

`topgrade -y`

- Cleanup temporary/old files:

`topgrade -c`

- Disable a certain update operation:

`topgrade --disable {{operation}}`

- Only perform a certain update operation:

`topgrade --only {{operation}}`

- Edit the config file with default editor:

`topgrade --edit-config`
