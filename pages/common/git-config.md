# git config 
## chatgpt 
The `git config` command is used to configure Git settings both globally and on a per-repository basis. 

Here's how the command works and what some of its key options are:

Syntax:
```
git config [--global] [<name>] [<value>]
```

- The `--global` flag can be included to set configuration options globally. This means that the changes will apply to all Git repositories on a given user account, rather than just the current repository.

- `<name>` represents the name of the configuration option you want to set or view. It can be any string value.

- `<value>` represents the value you want to set for the configuration option. This can also be any string value.

Key options:

1. `--list` - Lists all the configuration settings either globally or for the current repository.

2. `--global` - Sets the specified configuration globally rather than locally in the current repository.

3. `--unset` - Unsets the specified configuration option either globally or locally.

4. `--unset-all` - Unsets all values for the specified configuration option globally.

5. `--edit` - Opens the configuration file in a text editor, allowing you to edit the settings manually.

Some examples of setting Git configuration using the git config command are:
```
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
git config color.ui true

``` 

In the above examples, we use the `git config` command to set the user name and email globally and enable colored output. 

## tldr 
 
> Manage custom configuration options for Git repositories.
> These configurations can be local (for the current repository) or global (for the current user).
> More information: <https://git-scm.com/docs/git-config>.

- List only local configuration entries (stored in `.git/config` in the current repository):

`git config --list --local`

- List only global configuration entries (stored in `~/.gitconfig`):

`git config --list --global`

- List only system configuration entries (stored in `/etc/gitconfig`), and show their file location:

`git config --list --system --show-origin`

- Get the value of a given configuration entry:

`git config alias.unstage`

- Set the global value of a given configuration entry:

`git config --global alias.unstage "reset HEAD --"`

- Revert a global configuration entry to its default value:

`git config --global --unset alias.unstage`

- Edit the Git configuration for the current repository in the default editor:

`git config --edit`

- Edit the global Git configuration in the default editor:

`git config --global --edit`
