# guix package 
## chatgpt 
`guix package` is a command in the GNU Guix package manager that allows users to manage packages installed on their system.

It has several subcommands that perform different package management tasks, such as installing, upgrading, removing, and searching for packages. Here are some examples of the subcommands and their usage:

- `guix package search`: This subcommand allows you to search for packages in the Guix repository. For example, you can search for all available packages with the keyword "python" by running: `guix package search python`

- `guix package install`: This subcommand allows you to install packages from the Guix repository. For example, you can install the "python" package by running: `guix package install python`

- `guix package upgrade`: This subcommand allows you to upgrade installed packages to their latest version. For example, you can upgrade all packages on your system by running: `guix package upgrade`

- `guix package remove`: This subcommand allows you to remove installed packages from your system. For example, you can remove the "python" package by running: `guix package remove python`

Overall, `guix package` is a powerful tool for managing packages on a GNU Guix-based Linux system. 

## tldr 
 
> Install, upgrade and remove Guix packages, or rollback to previous configurations.
> More information: <https://guix.gnu.org/manual/html_node/Invoking-guix-package.html>.

- Install a new package:

`guix package -i {{package_name}}`

- Remove a package:

`guix package -r {{package_name}}`

- Search the package database for a regular expression:

`guix package -s "{{search_pattern}}"`

- List installed packages:

`guix package -I`

- List generations:

`guix package -l`

- Roll back to the previous generation:

`guix package --roll-back`
