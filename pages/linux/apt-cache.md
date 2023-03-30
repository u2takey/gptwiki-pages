# apt-cache 
## chatgpt 
`apt-cache` is a command-line utility tool in Linux for querying information about packages available in the system's configured APT repositories. APT is a package manager that helps in installing, updating and managing packages on Debian, Ubuntu and other similar Linux distributions.

The `apt-cache` command is used to search, retrieve, and display various cache data related to installed and available packages on the system. Some of the commonly used options for `apt-cache` command are:

- `search`: Searches the repository database for packages matching the given keyword pattern.
  - Syntax: `apt-cache search <keyword>`
- `show`: Displays detailed information about a package, such as its version, size, dependencies, and maintainer.
  - Syntax: `apt-cache show <package name>`
- `depends`: Displays the dependencies of a package, including a list of packages that the package depends on to function correctly.
  - Syntax: `apt-cache depends <package name>`
- `rdepends`: Displays the reverse dependencies of a package, including a list of packages that depend on the package specified as input.
  - Syntax: `apt-cache rdepends <package name>`
- `policy`: Displays the policy settings for a package, including information about its priority, version, and installed status.
  - Syntax: `apt-cache policy <package name>`

Overall, the `apt-cache` command is a useful tool for managing and troubleshooting packages on a Linux system. It can be used to search for packages, display their details, and inspect their dependencies, making it an essential tool for software developers, system administrators, and Linux users in general. 

## tldr 
 
> Debian and Ubuntu package query tool.
> More information: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

- Search for a package in your current sources:

`apt-cache search {{query}}`

- Show information about a package:

`apt-cache show {{package}}`

- Show whether a package is installed and up to date:

`apt-cache policy {{package}}`

- Show dependencies for a package:

`apt-cache depends {{package}}`

- Show packages that depend on a particular package:

`apt-cache rdepends {{package}}`
