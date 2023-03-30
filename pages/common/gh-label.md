# gh label 
## chatgpt 
As an AI language model, I don't have access to the context you're referring to. However, generally, the `gh label` command is a command-line interface tool provided by GitHub that allows you to manage labels for issues and pull requests in your repository. 

Here are some details about the command:

- `gh` is the command-line interface tool for GitHub. Depending on your system, you may need to install it separately.

- `label` is the subcommand that you add to the `gh` command to interact with issue and pull request labels.

- Running `gh label` on its own doesn't do anything; you need to add other subcommands and options to perform actions. Some examples of subcommands and options are:
  - `gh label list` will show you a list of all the labels in your repository.
  - `gh label create` allows you to create a new label for your repository.
  - `gh label edit` lets you edit an existing label.
  
The `gh label` command is a useful tool for managing labels in your GitHub projects, and provides a convenient way to make label-related changes directly from the command line. 

## tldr 
 
> Work with GitHub labels on the command-line.
> More information: <https://cli.github.com/manual/gh_label>.

- List labels for the repository in the current directory:

`gh label list`

- View labels for the repository in the current directory in the default web browser:

`gh label list --web`

- Create a label with a specific name, description and color in hexadecimal format for the repository in the current directory:

`gh label create {{name}} --description "{{description}}" --color {{color_hex}}`

- Delete a label for the repository in the current directory, prompting for confirmation:

`gh label delete {{name}}`

- Update the name and description for a specific label for the repository in the current directory:

`gh label edit {{name}} --name {{new_name}} --description "{{description}}"`

- Clone labels from a specific repository into the repository in the current directory:

`gh label clone {{owner}}/{{repository}}`

- Display help for a subcommand:

`gh label {{subcommand}} --help`
