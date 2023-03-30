# nodenv 
## chatgpt 
nodenv is a command-line utility used for managing and switching between different versions of Node.js on a single machine. It allows developers to switch between different versions of Node.js on a per-project basis or globally. Nodenv also provides a way to install and manage Node.js versions using a plugin system.

Some of the common commands used with nodenv are:

1. nodenv versions: Displays a list of all the installed Node.js versions.

2. nodenv install: Used to install a specific version of Node.js on the system.

3. nodenv local: Used to set a local Node.js version for a specific project. This command will create a .node-version file in the project directory, which specifies the Node.js version to use.

4. nodenv global: Used to set the default global Node.js version for the system.

5. nodenv rehash: Used to update the PATH environment to include the bin directories of the installed Node.js versions.

Using nodenv, developers can easily switch between different versions of Node.js without having to worry about conflicts or compatibility issues between different projects. It's a powerful tool that can improve the productivity of Node.js developers significantly. 

## tldr 
 
> A tool to manage Node.js versions.
> More information: <https://github.com/nodenv/nodenv>.

- Install a specific version of Node.js:

`nodenv install {{version}}`

- Display a list of available versions:

`nodenv install --list`

- Use a specific version of Node.js across the whole system:

`nodenv global {{version}}`

- Use a specific version of Node.js with a directory:

`nodenv local {{version}}`

- Display the Node.js version for the current directory:

`nodenv version`

- Display the location of a Node.js installed command (e.g. `npm`):

`nodenv which {{command}}`
