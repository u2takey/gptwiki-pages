# rbenv 
## chatgpt 
rbenv is a command-line tool used to manage multiple Ruby versions on a single machine. It allows users to install, uninstall, and switch between different versions of Ruby, as well as manage Ruby dependencies and project-specific Ruby versions.

Here is a brief overview of some common rbenv commands:

- `rbenv versions`: Lists all installed versions of Ruby.
- `rbenv install <version>`: Installs a specific version of Ruby.
- `rbenv global <version>`: Sets the global version of Ruby to use as default.
- `rbenv local <version>`: Sets the local version of Ruby to use for a specific project's directory.
- `rbenv shell <version>`: Sets the current shell session to use a specific version of Ruby.
- `rbenv rehash`: Updates the command-line tools to use the current version of Ruby.
- `rbenv which <command>`: Shows the location of the command in the current Ruby environment.

Overall, rbenv is a powerful tool for managing multiple Ruby versions and dependencies, and can greatly simplify the task of working with different Ruby projects on a single machine. 

## tldr 
 
> A tool to easily install Ruby versions and manage application environments.
> More information: <https://github.com/rbenv/rbenv>.

- Install a Ruby version:

`rbenv install {{version}}`

- Display a list of the latest stable versions for each Ruby:

`rbenv install --list`

- Display a list of installed Ruby versions:

`rbenv versions`

- Use a specific Ruby version across the whole system:

`rbenv global {{version}}`

- Use a specific Ruby version for an application/project directory:

`rbenv local {{version}}`

- Display the currently selected Ruby version:

`rbenv version`

- Uninstall a Ruby version:

`rbenv uninstall {{version}}`

- Display all Ruby versions that contain the specified executable:

`rbenv whence {{executable}}`
