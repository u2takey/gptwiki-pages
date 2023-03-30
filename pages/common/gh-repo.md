# gh repo 
## chatgpt 
gh repo is a command that provides a shortcut for various actions related to GitHub repositories. The command is used with different subcommands to perform various actions related to repositories.

Some of the commonly used subcommands of gh repo are:

- create: This subcommand is used to create a new GitHub repository from the command line. It prompts the user for the repository name, description, public or private visibility, and other options, and creates the repository in the user's GitHub account.

- view: This subcommand is used to view the details of a GitHub repository from the command line. It shows the repository name, description, owner, creation date, last updated date, and other details.

- clone: This subcommand is used to clone a GitHub repository to the local machine. It creates a copy of the repository in the user's local directory, and sets up the necessary git configuration and remote repository.

- fork: This subcommand is used to create a fork of an existing GitHub repository. It creates a copy of the repository in the user's GitHub account, and sets up the necessary git configuration and remote repository.

- delete: This subcommand is used to delete a GitHub repository from the command line. It prompts the user for confirmation before deleting the repository, and also offers an option to transfer the repository to another user or organization.

Overall, gh repo provides a convenient and streamlined way to manage GitHub repositories from the command line, without having to switch to the GitHub web interface. 

## tldr 
 
> Work with GitHub repositories on the command-line.
> More information: <https://cli.github.com/manual/gh_repo>.

- Create a new repository (if the repository name is not set, the default name will be the name of the current directory):

`gh repo create {{name}}`

- Clone a repository:

`gh repo clone {{owner}}/{{repository}}`

- Fork and clone a repository:

`gh repo fork {{owner}}/{{repository}} --clone`

- View a repository in the default web browser:

`gh repo view {{repository}} --web`

- List repositories owned by a specific user or organization (if the owner is not set, the default owner will be the currently logged in user):

`gh repo list {{owner}}`

- List only non-forks repositories:

`gh repo list {{owner}} --non-forks`

- List repositories with a specific primary coding language:

`gh repo list {{owner}} --language {{language_name}}`
