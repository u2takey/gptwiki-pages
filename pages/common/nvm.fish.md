# nvm 
## chatgpt 
nvm stands for Node Version Manager. It is a command-line tool that allows you to install, manage, and switch between multiple versions of Node.js on your machine.

Here are some of the commands you can use with nvm:

- nvm install [version]: This command installs the specified version of Node.js. For example, you can run `nvm install 12.18.3` to install Node.js version 12.18.3.

- nvm use [version]: This command switches to the specified version of Node.js. For example, you can run `nvm use 12.18.3` to switch to version 12.18.3.

- nvm ls: This command lists all the versions of Node.js that are installed on your machine.

- nvm alias [name] [version]: This command creates an alias for a specific version of Node.js. For example, you can run `nvm alias default 12.18.3` to set the default version to 12.18.3.

- nvm current: This command displays the currently active version of Node.js.

Overall, nvm is a useful tool for developers who need to work with different versions of Node.js for different projects. 

## tldr 
 
> Install, uninstall, or switch between Node.js versions under the `fish` shell.
> Supports version numbers like "12.8" or "v16.13.1", and labels like "stable", "system", etc.
> More information: <https://github.com/jorgebucaran/nvm.fish>.

- Install a specific version of Node.js:

`nvm install {{node_version}}`

- Use a specific version of Node.js in the current shell:

`nvm use {{node_version}}`

- Set the default Node.js version:

`set nvm_default_version {{node_version}}`

- List all available Node.js versions and highlight the default one:

`nvm list`

- Uninstall a given Node.js version:

`nvm uninstall {{node_version}}`
