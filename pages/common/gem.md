# gem 
## chatgpt 
`gem` is a command-line tool that comes with RubyGems, a package manager for the Ruby programming language. 

The `gem` command allows you to manage RubyGems, such as installing, updating, and removing RubyGems, as well as listing installed RubyGems and their dependencies. 

Here are some common gem commands:

- `gem install [gemname]`: installs the specified RubyGem
- `gem list`: lists all installed RubyGems
- `gem update [gemname]`: updates the specified RubyGem to the latest version
- `gem uninstall [gemname]`: uninstalls the specified RubyGem
- `gem search [searchterm]`: searches for RubyGems that match the specified search term
- `gem info [gemname]`: displays information about the specified RubyGem

There are many other options and subcommands available for the `gem` command, which you can explore by running `gem help`. 

## tldr 
 
> Interact with the package manager for the Ruby programming language.
> More information: <https://rubygems.org>.

- Search for remote gem(s) and show all available versions:

`gem search {{regular_expression}} --all`

- Install the latest version of a gem:

`gem install {{gemname}}`

- Install specific version of a gem:

`gem install {{gemname}} --version {{1.0.0}}`

- Install the latest matching (SemVer) version of a gem:

`gem install {{gemname}} --version '~> {{1.0}}'`

- Update a gem:

`gem update {{gemname}}`

- List all local gems:

`gem list`

- Uninstall a gem:

`gem uninstall {{gemname}}`

- Uninstall specific version of a gem:

`gem uninstall {{gemname}} --version {{1.0.0}}`
