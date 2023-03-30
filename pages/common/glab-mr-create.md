# glab mr create 
## chatgpt 
The `glab mr create` command is used to create a new merge request in GitLab. It is executed in the command-line interface (CLI) or terminal.

The `glab` command stands for GitLab CLI, which is an interface that allows users to interact with GitLab repositories through the terminal.

The `mr` is an abbreviation for merge request, and the `create` subcommand is used to create a new merge request.

When executing the `glab mr create` command, you will be prompted to provide information related to the new merge request, such as the source branch, target branch, title, description, and assignee. Once you have provided all the required information, GitLab will automatically create a new merge request based on your inputs.

Overall, the `glab mr create` command provides a quick and easy way to create new merge requests in GitLab through the command-line interface. 

## tldr 
 
> Manage GitLab merge requests from the command-line.
> More information: <https://glab.readthedocs.io/en/latest/mr/create.html>.

- Interactively create a merge request:

`glab mr create`

- Create a merge request, determining the title and description from the commit messages of the current branch:

`glab mr create --fill`

- Create a draft merge request:

`glab mr create --draft`

- Create a merge request specifying the target branch, title, and description:

`glab mr create --target-branch {{target_branch}} --title "{{title}}" --description "{{description}}"`

- Start opening a merge request in the default web browser:

`glab mr create --web`
