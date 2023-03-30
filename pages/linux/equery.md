# equery 
## chatgpt 
equery is a command-line utility that is used to query the Gentoo package database. It allows users to obtain detailed information about installed packages, as well as search the repository for available packages. The equery command can be used with a number of different subcommands, each of which serves a specific purpose.

Some of the commonly used subcommands of equery are:

1. `equery list`: This subcommand is used to list all the installed packages on the system. By default, it shows the package name and version number.

2. `equery uses`: This subcommand is used to show the dependencies of a package.

3. `equery depends`: This subcommand is used to show the reverse dependencies of a package.

4. `equery files`: This subcommand is used to list all the files installed by a package.

5. `equery check`: This subcommand is used to check the integrity of the files installed by a package.

6. `equery belongs`: This subcommand is used to find the package which owns a specific file.

7. `equery hasuse`: This subcommand is used to check if a package has a specific USE flag enabled.

8. `equery size`: This subcommand is used to show the size of the package and its dependencies.

Overall, equery is a powerful tool that allows users to interact with the Gentoo package database in a variety of ways. It can help users to manage their installed packages, troubleshoot issues related to dependencies, and more. 

## tldr 
 
> View information about Portage packages.
> More information: <https://wiki.gentoo.org/wiki/Equery>.

- List all installed packages:

`equery list '*'`

- Search for installed packages in the Portage tree and in overlays:

`equery list -po {{package_name}}`

- List all packages that depend on a given package:

`equery depends {{package_name}}`

- List all packages that a given package depends on:

`equery depgraph {{package_name}}`

- List all files installed by a package:

`equery files --tree {{package_name}}`
