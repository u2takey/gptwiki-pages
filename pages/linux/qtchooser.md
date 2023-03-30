# qtchooser 
## chatgpt 
Qtchooser is a command-line tool that is used to manage and switch between different versions of the Qt development libraries and tools. It is typically included in Qt installations on Linux and Unix systems and is used to assist with managing multiple installed versions of the Qt development software.

The qtchooser command provides a number of options that can be used to list available Qt versions, set the default version to use, or even run Qt applications with a specific version of the Qt libraries. Some common options that can be used with the qtchooser command include:

- `--list-versions`: This option lists all available Qt versions that are currently installed on the system.

- `--print-env`: This option prints the environment variables that are set by qtchooser based on the currently selected Qt version.

- `--query`: This option can be used to query information about a specific Qt version, such as the path to the Qt installation or the location of the qmake tool.

- `--run-tool`: This option allows you to run a specific Qt tool, such as qmake or qtconfig, with the selected Qt version.

Overall, the qtchooser command is a useful tool for managing multiple versions of the Qt development software on a Linux or Unix system, and provides a flexible way to customize your development environment based on your specific needs. 

## tldr 
 
> A wrapper used to select between Qt development binary versions.
> More information: <https://manned.org/qtchooser>.

- List available Qt versions from the configuration files:

`qtchooser --list-versions`

- Print environment information:

`qtchooser --print-env`

- Run the specified tool using the specified Qt version:

`qtchooser --run-tool={{tool}} --qt={{version_name}}`

- Add a Qt version entry to be able to choose from:

`qtchooser --install {{version_name}} {{path/to/qmake}}`

- Display all available options:

`qtchooser --help`
