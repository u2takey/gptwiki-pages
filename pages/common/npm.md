# npm 
## chatgpt 
npm (short for Node Package Manager) is a command-line tool that is used to install and manage packages (i.e. libraries, frameworks, and other software dependencies) for Node.js projects. 

The npm command provides a variety of functions, including:

1. Installing packages - this is done with the `npm install` command, followed by the name of the package(s) you want to install. For example, `npm install express` would install the Express framework for Node.js.

2. Managing packages - you can use `npm update` to update any packages that you have installed to their latest version. You can also use `npm uninstall` to remove packages that you no longer need.

3. Running scripts - npm supports the execution of scripts defined in the project's `package.json` file by running the command `npm run` followed by the script name.

4. Publishing packages - npm allows you to publish your own packages to the npm registry so that others can use them. This is done using the `npm publish` command, but requires an account on the registry.

Overall, npm is a powerful tool for managing Node.js projects, allowing developers to easily manage and install dependencies as well as automate tasks with scripts. 

## tldr 
 
> JavaScript and Node.js package manager.
> Manage Node.js projects and their module dependencies.
> More information: <https://www.npmjs.com>.

- Interactively create a `package.json` file:

`npm init`

- Download all the packages listed as dependencies in package.json:

`npm install`

- Download a specific version of a package and add it to the list of dependencies in `package.json`:

`npm install {{module_name}}@{{version}}`

- Download a package and add it to the list of dev dependencies in `package.json`:

`npm install {{module_name}} --save-dev`

- Download a package and install it globally:

`npm install --global {{module_name}}`

- Uninstall a package and remove it from the list of dependencies in `package.json`:

`npm uninstall {{module_name}}`

- Print a tree of locally installed dependencies:

`npm list`

- List top-level globally installed modules:

`npm list --global --depth={{0}}`
