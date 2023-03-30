# nvm 
## chatgpt 
`nvm` stands for Node Version Manager. It is a software tool used to manage multiple versions of Node.js installed on a single machine.

Using `nvm`, developers can:

- Install and switch between multiple versions of Node.js on their machine.
- Use the latest LTS (Long Term Support) release of Node.js for stable applications.
- Test their code with different versions of Node.js without needing to uninstall and reinstall each time.
- Easily manage their Node.js environment without affecting other applications on the same machine.

Some common commands used in `nvm` are:

- `nvm install [version]`: installs a specific version of Node.js.
- `nvm use [version]`: switches the current terminal session to use the specified version of Node.js.
- `nvm list`: displays a list of all installed versions of Node.js.
- `nvm alias [name] [version]`: creates an alias for a specific Node.js version using a name of your choice.

Overall, `nvm` is a useful tool for managing Node.js environments and simplifying development across multiple projects. 

## tldr 
 
> Install, uninstall or switch between Node.js versions.
> Supports version numbers like "12.8" or "v16.13.1", and labels like "stable", "system", etc.
> More information: <https://github.com/creationix/nvm>.

- Install a specific version of Node.js:

`nvm install {{node_version}}`

- Use a specific version of Node.js in the current shell:

`nvm use {{node_version}}`

- Set the default Node.js version:

`nvm alias default {{node_version}}`

- List all available Node.js versions and highlight the default one:

`nvm list`

- Uninstall a given Node.js version:

`nvm uninstall {{node_version}}`

- Launch the REPL of a specific version of Node.js:

`nvm run {{node_version}} --version`

- Execute a script in a specific version of Node.js:

`nvm exec {{node_version}} node {{app.js}}`
