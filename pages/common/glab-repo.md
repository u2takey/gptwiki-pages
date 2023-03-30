# glab repo 
## chatgpt 
The glab repo command is a command-line interface (CLI) tool that is used with GitLab to manage repositories. The glab repo command allows you to perform various operations on repositories, such as creating, deleting, cloning, fetching, pushing, and more. 

Here is an overview of the different subcommands available with the glab repo command: 

- `glab repo clone`: This subcommand is used to clone a remote repository to a local system. 

- `glab repo create`: This subcommand is used to create a new repository on GitLab. 

- `glab repo delete`: This subcommand is used to delete a GitLab repository. 

- `glab repo fetch`: This subcommand is used to fetch updates from the remote repository. 

- `glab repo fork`: This subcommand is used to creates a fork of a project in your namespace. 

- `glab repo list`: This subcommand is used to list all the repositories available in a user, group or organization account. 

- `glab repo push`: This subcommand is used to push code changes to a remote repository. 

- `glab repo rename`: This subcommand is used to rename a repository. 

- `glab repo transfer`: This subcommand is used to transfer ownership of a repository to a different user, group or organization account.

In summary, the glab repo command is a powerful tool that allows developers to manage their GitLab repositories efficiently from the command line interface. 

## tldr 
 
> Work with GitLab repositories on the command-line.
> More information: <https://glab.readthedocs.io/en/latest/repo/index.html#synopsis>.

- Create a new repository (if the repository name is not set, the default name will be the name of the current directory):

`glab repo create {{name}}`

- Clone a repository:

`glab repo clone {{owner}}/{{repository}}`

- Fork and clone a repository:

`glab repo fork {{owner}}/{{repository}} --clone`

- View a repository in the default web browser:

`glab repo view {{owner}}/{{repository}} --web`

- Search some repositories in the GitLab instance:

`glab repo search -s {{search_string}}`
