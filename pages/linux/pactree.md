# pactree 
## chatgpt 
The `pactree` command is a utility program used in Arch Linux and its derivatives to display a tree view of the dependencies of a particular package. Here's a detailed explanation of the command:

Usage: `pactree [options] [package name]`

Options:

- `-h`: Displays the help message and a list of available options.
- `-l`: Generates a list of packages that depend on the target package.
- `-r`: Includes packages that are required by the target package, but not included in its dependencies. This is useful when you want to see the full tree of dependencies, including indirect ones.

Package name:

- This is the name of the package you want to view the dependencies of. If no package name is specified, `pactree` will show the dependencies for all installed packages.

Functionality:

- When you run the `pactree` command on a package, it displays a tree view of its dependencies. The package you chose is at the top, and its direct dependencies are listed beneath it. If you used the `-r` option, indirect dependencies will also be included.
- Packages in bold are required by the target package, while regular packages are only recommended or optional dependencies.
- When used with the `-l` option, `pactree` will display a list of packages that depend on the target package, rather than its dependencies.

Example:

- To view the dependencies of a package named `firefox`, you can run `pactree firefox` in the terminal. This will show you a tree view of Firefox's dependencies.
- If you instead want to see a list of packages that depend on Firefox, you can run `pactree -l firefox`. This will show you a list of packages that require or recommend Firefox. 

## tldr 
 
> Package dependency tree viewer for pacman.
> More information: <https://man.archlinux.org/man/pactree.8>.

- Print the dependency tree of a specific package:

`pactree {{package}}`

- Print what packages depend on a specific package:

`pactree --reverse {{package}}`

- Dump dependencies one per line, skipping duplicates:

`pactree --unique {{package}}`

- Include optional dependencies of a specific package and colorize the output:

`pactree --optional --color {{package}}`

- Display help:

`pactree`
