# dotnet restore 
## chatgpt 
The "dotnet restore" command is a command-line utility used in the .NET Core SDK to restore dependencies for a .NET Core application.

When a .NET Core application is built using the "dotnet build" command or a package is added through the "dotnet add package" command, the dependencies for the application or package are listed in a file called the "project file" (typically a .csproj file). The "dotnet restore" command reads this project file and installs all necessary dependencies required for the project in the local machine's cache.

When the command is executed, the following actions happen:

1. The command reads the project file(s) and determines the dependencies required for the project.

2. It then checks the local cache for each dependency.

3. If the dependency is not found in the local cache, it downloads the dependency from the configured package sources (such as NuGet) and installs it in the local cache.

4. If the dependency has already been installed in the cache, it verifies if there are any updates available for the installed dependencies and updates them if necessary.

In summary, the "dotnet restore" command ensures that all the necessary dependencies for a .NET Core project are installed and updated as required, making it easier to build and run the project. 

## tldr 
 
> Restores the dependencies and tools of a .NET project.
> More information: <https://learn.microsoft.com/dotnet/core/tools/dotnet-restore>.

- Restore dependencies for a .NET project or solution in the current directory:

`dotnet restore`

- Restore dependencies for a .NET project or solution in a specific location:

`dotnet restore {{path/to/project_or_solution}}`

- Restore dependencies without caching the HTTP requests:

`dotnet restore --no-cache`

- Force all dependencies to be resolved even if the last restore was successful:

`dotnet restore --force`

- Restore dependencies using package source failures as warnings:

`dotnet restore --ignore-failed-sources`

- Restore dependencies with a specific verbosity level:

`dotnet restore --verbosity {{quiet|minimal|normal|detailed|diagnostic}}`
