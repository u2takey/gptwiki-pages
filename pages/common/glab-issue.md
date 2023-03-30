# glab issue 
## chatgpt 
The `glab issue` command is a GitLab command-line interface (CLI) command that allows users to manage issues within a GitLab project. The command provides several subcommands that can be used to create, view, update, and close issues.

Syntax: `glab issue [subcommand] [flags]`

Some of the subcommands available under `glab issue` are:

1. `create`: This subcommand creates a new issue in a GitLab project. Users can provide details such as the issue title, description, milestone, labels, and assignee.

Syntax: `glab issue create [flags]`

2. `list`: This subcommand lists all the issues in a GitLab project. Users can use filters such as milestone, label, and assignee to refine the results.

Syntax: `glab issue list [flags]`

3. `open`: This subcommand opens an existing issue in a GitLab project.

Syntax: `glab issue open [flags]`

4. `close`: This subcommand closes an existing issue in a GitLab project.

Syntax: `glab issue close [flags]`

There are several other subcommands available under `glab issue`, such as `edit`, `comment`, and `delete`. The command also provides several flags that can be used to specify additional details or filters.

Overall, the `glab issue` command is a powerful tool for managing issues within a GitLab project from the command line. 

## tldr 
 
> Manage GitLab issues from the command-line.
> More information: <https://glab.readthedocs.io/en/latest/issue>.

- Display a specific issue:

`glab issue view {{issue_number}}`

- Display a specific issue in the default web browser:

`glab issue view {{issue_number}} --web`

- Create a new issue in the default web browser:

`glab issue create --web`

- List the last 10 issues with the `bug` label:

`glab issue list --per-page {{10}} --label "{{bug}}"`

- List closed issues made by a specific user:

`glab issue list --closed --author {{username}}`

- Reopen a specific issue:

`glab issue reopen {{issue_number}}`
