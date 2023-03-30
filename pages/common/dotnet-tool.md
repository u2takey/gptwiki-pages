# dotnet tool 
## chatgpt 
The `dotnet tool` command is a command-line interface (CLI) tool that is part of the .NET Core SDK. It allows users to manage .NET Core command-line tools that are installed on their local machine.

Here are the details of the subcommands that can be used with the `dotnet tool` command:

- `dotnet tool install`: Installs a .NET Core command-line tool on the local machine. Users can specify the tool name, version, source, and other options.

- `dotnet tool list`: Lists all the installed .NET Core command-line tools on the local machine.

- `dotnet tool uninstall`: Uninstalls a .NET Core command-line tool on the local machine. Users can specify the tool name, version, and other options.

- `dotnet tool update`: Updates a .NET Core command-line tool on the local machine to the latest version.

- `dotnet tool restore`: Restores the NuGet packages for the .NET Core command-line tool project.

- `dotnet tool run`: Runs a .NET Core command-line tool on the local machine. Users can specify the tool name, arguments, and other options.

Using the `dotnet tool` command, developers can easily manage their .NET Core tools on their local machine, which helps to simplify the development process. 

## tldr 
 
> Manage .NET tools and search published tools in NuGet.
> More information: <https://learn.microsoft.com/dotnet/core/tools/global-tools>.

- Install a global tool (don't use `--global` for local tools):

`dotnet tool install --global {{dotnetsay}}`

- Install tools defined in the local tool manifest:

`dotnet tool restore`

- Update a specific global tool (don't use `--global` for local tools):

`dotnet tool update --global {{tool_name}}`

- Uninstall a global tool (don't use `--global` for local tools):

`dotnet tool uninstall --global {{tool_name}}`

- List installed global tools (don't use `--global` for local tools):

`dotnet tool list --global`

- Search tools in NuGet:

`dotnet tool search {{search_term}}`

- Display help:

`dotnet tool --help`
