# nvm 
## chatgpt 
`nvm` stands for Node Version Manager. It is a command-line tool that enables you to manage multiple versions of Node.js, which is a popular runtime environment that allows developers to use JavaScript outside of a web browser, such as creating server-side applications.

With `nvm`, you can install and switch between different versions of Node.js on your computer. This is useful when working on projects that require specific Node.js versions, or when you want to test your code with different runtime environments.

Here are some common `nvm` commands:

- `nvm ls`: list all the installed versions of Node.js on your system
- `nvm install <version>`: install a specific version of Node.js (e.g. `nvm install 14.17.3`)
- `nvm use <version>`: switch to a specific version of Node.js for your current shell session (e.g. `nvm use 14.17.3`)
- `nvm default <version>`: set a specific version of Node.js as your default version

`nvm` is available on Unix-based systems (such as macOS and Linux), as well as on Windows using a Bash emulator like Git Bash or Windows Subsystem for Linux (WSL). 

## tldr 
 
> Install, uninstall, or switch between Node.js versions.
> Supports version numbers like "12.8" or "v16.13.1", and labels like "stable", "system", etc.
> More information: <https://github.com/coreybutler/nvm-windows>.

- Install a specific version of Node.js:

`nvm install {{node_version}}`

- Set the default version of Node.js (must be run as Administrator):

`nvm use {{node_version}}`

- List all available Node.js versions and highlight the default one:

`nvm list`

- List all remote Node.js versions:

`nvm ls-remote`

- Uninstall a given Node.js version:

`nvm uninstall {{node_version}}`
