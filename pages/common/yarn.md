# yarn 
## chatgpt 
Yarn is a package manager for node.js that was created by Facebook developers. It allows users to manage node modules and dependencies in their projects.

The `yarn` command is the basic command used to interact with the package manager. Running `yarn` in the terminal will execute the following steps:

1. Check for the existence of `package.json` file in the current directory. This file is used to track the dependencies and metadata of the current project.
2. If `package.json` is present, Yarn will read its contents to regenerate `yarn.lock` file which lists all the modules and their dependencies being used in the project. If `yarn.lock` already exists, the file is updated with only the required changes.
3. If `package.json` is not present, Yarn will initialize a new project by creating a default `package.json` file.
4. Once the `yarn.lock` file is updated, Yarn will install any new dependencies or update pre-existing ones (if needed) by downloading the specified version(s) of each module listed in the `yarn.lock` file.
5. If post-install scripts are declared in the `package.json` file, Yarn will run those scripts after installing the dependencies.

Overall, the `yarn` command is the backbone of Yarn's functionality, as it manages the installation and updating of dependencies for any given node.js project. 

## tldr 
 
> JavaScript and Node.js package manager alternative.
> More information: <https://yarnpkg.com>.

- Install a module globally:

`yarn global add {{module_name}}`

- Install all dependencies referenced in the `package.json` file (the `install` is optional):

`yarn install`

- Install a module and save it as a dependency to the `package.json` file (add `--dev` to save as a dev dependency):

`yarn add {{module_name}}@{{version}}`

- Uninstall a module and remove it from the `package.json` file:

`yarn remove {{module_name}}`

- Interactively create a `package.json` file:

`yarn init`

- Identify whether a module is a dependency and list other modules that depend upon it:

`yarn why {{module_name}}`
