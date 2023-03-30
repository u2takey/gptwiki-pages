# gh issue 
## chatgpt 
The "gh issue" command is a command that is commonly used in GitHub CLI (Command Line Interface) to interact with issues within GitHub repositories. This command can be used to view, create, update, and close issues within a repository.

Here are some of the main sub-commands that can be used with "gh issue" and what they do:

1. gh issue list: This sub-command is used to list all the issues in the current repository. It displays information about each issue, such as its title, number, status, and assignees.

2. gh issue view: This sub-command is used to view the details of a specific issue. It displays more detailed information about the issue, including its description, comments, labels, and milestones.

3. gh issue create: This sub-command is used to create a new issue in the current repository. It prompts the user to provide information about the issue, such as its title, description, and labels.

4. gh issue edit: This sub-command is used to edit an existing issue in the current repository. It prompts the user to make changes to the issue's title, description, labels, and other properties.

5. gh issue close: This sub-command is used to close an existing issue in the current repository. It sets the issue's status to "closed" and adds a comment indicating that the issue has been resolved.

6. gh issue reopen: This sub-command is used to reopen a closed issue in the current repository. It sets the issue's status back to "open" and removes the comment that was added when the issue was closed.

Overall, the "gh issue" command is a powerful tool for managing issues in GitHub repositories from the command line. It can help users quickly view, create, and update issues without needing to navigate to GitHub's web interface. 

## tldr 
 
> Manage GitHub issues from the command-line.
> More information: <https://cli.github.com/manual/gh_issue>.

- Display a specific issue:

`gh issue view {{issue_number}}`

- Display a specific issue in the default web browser:

`gh issue view {{issue_number}} --web`

- Create a new issue in the default web browser:

`gh issue create --web`

- List the last 10 issues with the `bug` label:

`gh issue list --limit {{10}} --label "{{bug}}"`

- List closed issues made by a specific user:

`gh issue list --state closed --author {{username}}`

- Display the status of issues relevant to the user, in a specific repository:

`gh issue status --repo {{owner}}/{{repository}}`

- Reopen a specific issue:

`gh issue reopen {{issue_number}}`
