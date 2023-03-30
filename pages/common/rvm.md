# rvm 
## chatgpt 
rvm is a command-line tool that stands for Ruby Version Manager. It is used to manage and install different versions of Ruby on your system.

When the user types in "rvm" in the terminal, they will see a list of available commands and options. These commands can be used to switch between different versions of Ruby, install new versions of Ruby, and even manage Gemsets, which are groups of gems that can be used for different Ruby projects.

Some of the most common commands used with rvm include:

- `rvm list`: Lists all the installed versions of Ruby on your system
- `rvm use [ruby-version]`: Switches the Ruby version to the specified version
- `rvm install [ruby-version]`: Installs a new version of Ruby
- `rvm gemset create [gemset-name]`: Creates a new Gemset
- `rvm gemset use [gemset-name]`: Switches to the specified Gemset

Overall, rvm is a useful tool for developers who need to manage multiple versions of Ruby on their system. 

## tldr 
 
> A tool for easily installing, managing, and working with multiple ruby environments.
> More information: <https://rvm.io>.

- Install one or more space-separated versions of Ruby:

`rvm install {{version(s)}}`

- Display a list of installed versions:

`rvm list`

- Use a specific version of Ruby:

`rvm use {{version}}`

- Set the default Ruby version:

`rvm --default use {{version}}`

- Upgrade a version of Ruby to a new version:

`rvm upgrade {{current_version}} {{new_version}}`

- Uninstall a version of Ruby and keep its sources:

`rvm uninstall {{version}}`

- Remove a version of Ruby and its sources:

`rvm remove {{version}}`

- Show specific dependencies for your OS:

`rvm requirements`
