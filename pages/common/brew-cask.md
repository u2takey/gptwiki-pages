# brew --cask 
## chatgpt 
Brew is a package manager for macOS that simplifies the installation of software and command-line tools. It uses a command-line interface to install, update, and manage packages.

The `--cask` option of the `brew` command specifies that the package being installed is a cask package. A cask is a type of package that is focused on installing graphical user interface (GUI) applications on macOS.

Casks are usually installed in the `/Applications` directory, just like standard macOS applications. This makes it easier to manage and launch these applications as they appear in the user's Launchpad and Applications menu.

To use this option, you need to have the Homebrew Cask extension installed. This extension adds support for cask packages to Homebrew.

For example, to install the Google Chrome browser using brew and cask, you would run the following command:

```
brew cask install google-chrome
```

This would download the Google Chrome installer package and run it, installing the browser on your mac. 

## tldr 
 
> CLI workflow for the administration of macOS applications distributed as binaries.
> This command was previously called `brew cask`, it has been deprecated in favor of the `brew --cask` flag.
> More information: <https://github.com/Homebrew/homebrew-cask>.

- Search for formulas and casks:

`brew search {{text}}`

- Install a cask:

`brew install --cask {{cask_name}}`

- List all installed casks:

`brew list --cask`

- List installed casks that have newer versions available:

`brew outdated --cask`

- Upgrade an installed cask (if no cask name is given, all installed casks are upgraded):

`brew upgrade --cask {{cask_name}}`

- Uninstall a cask:

`brew uninstall --cask {{cask_name}}`

- Uninstall a cask and remove related settings and files:

`brew zap --cask {{cask_name}}`

- Display information about a given cask:

`brew info --cask {{cask_name}}`
