# pnpm 
## chatgpt 
`pnpm` is a command-line tool that is used for managing Node.js dependencies. It stands for "performant npm" and is an alternative to the traditional `npm` package manager. This tool provides some added benefits compared to `npm`, such as faster installation times, disk space optimization, and version-locking.

Here are some of the key commands and their descriptions for `pnpm`:

- `pnpm install`: This command is the equivalent of `npm install`. It installs all the required dependencies for a project according to the information found in the package.json file. 

- `pnpm add`: This command is used to install a new package and add it to the list of dependencies in package.json.

- `pnpm update`: This command updates all the packages to their latest versions. 

- `pnpm remove`: This command is used to remove a package from the list of dependencies in package.json.

- `pnpm ls`: This command lists all the installed packages and their dependencies in a tree-like format.

- `pnpm run`: This command is similar to `npm run` and is used to run scripts defined in the scripts section of package.json.

- `pnpm test`: This command is used to run test scripts defined in the scripts section of package.json.

Overall, `pnpm` provides an alternative, faster approach to installing and managing Node.js dependencies, with easy access to various other helpful commands, as outlined above. 

## tldr 
 
> Fast, disk space efficient package manager for Node.js.
> Manage Node.js projects and their module dependencies.
> More information: <https://pnpm.io>.

- Create a `package.json` file:

`pnpm init`

- Download all the packages listed as dependencies in `package.json`:

`pnpm install`

- Download a specific version of a package and add it to the list of dependencies in `package.json`:

`pnpm add {{module_name}}@{{version}}`

- Download a package and add it to the list of [D]ev dependencies in `package.json`:

`pnpm add -D {{module_name}}`

- Download a package and install it [g]lobally:

`pnpm add -g {{module_name}}`

- Uninstall a package and remove it from the list of dependencies in `package.json`:

`pnpm remove {{module_name}}`

- Print a tree of locally installed modules:

`pnpm list`

- List top-level [g]lobally installed modules:

`pnpm list -g --depth={{0}}`
