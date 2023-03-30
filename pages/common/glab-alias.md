# glab alias 
## chatgpt 
The `glab alias` command is used in the GitLab command-line interface (CLI) to define custom aliases for commonly used GitLab commands. 

An alias is a custom command that you can create that represents one or more GitLab commands. It allows you to simplify complex commands into shorter and simpler commands that are easier to remember and type. Aliases can also help to standardize and automate commands across teams.

The syntax for the `glab alias` command is:

```
glab alias <alias-name> <command>
```

The `alias-name` parameter is the name of the alias you want to create, and the `command` parameter is the actual GitLab command that you want to represent with this alias.

For example, you could create an alias called "mrs" that represents the command "glab merge-request list":

```
glab alias mrs "merge-request list"
```

Now, instead of typing the long command "glab merge-request list" every time you want to list merge requests, you can simply type "glab mrs" to run the command.

You can also create more complex aliases that include multiple commands, options, or arguments. For example, you could create an alias that runs a script to clone a specific GitLab repository, and then opens it in your default editor:

```
glab alias myrepo "!(glab clone gitlab.com/myusername/myrepo && cd myrepo && code .)"
```

In this example, the alias "myrepo" runs two GitLab commands ("glab clone" and "cd"), and then opens the repository in the default editor with the "code" command.

Overall, the `glab alias` command is a useful tool for creating custom commands that can help to streamline your workflow and make working with GitLab more efficient. 

## tldr 
 
> Manage GitLab CLI command aliases from the command-line.
> More information: <https://glab.readthedocs.io/en/latest/alias>.

- Display the subcommand help:

`glab alias`

- List all the aliases `glab` is configured to use:

`glab alias list`

- Create a `glab` subcommand alias:

`glab alias set {{mrv}} '{{mr view}}'`

- Set a shell command as a `glab` subcommand:

`glab alias set --shell {{alias_name}} {{command}}`

- Delete a command shortcut:

`glab alias delete {{alias_name}}`
