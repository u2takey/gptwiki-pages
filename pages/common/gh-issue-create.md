# gh issue create 
## chatgpt 
The command `gh issue create` creates a new issue on a GitHub repository using the command-line interface (CLI) provided by the GitHub CLI tool.

Here's a breakdown of the command's individual parts:

- `gh` refers to the GitHub CLI tool. This is the program through which we'll be running the `issue create` command.
- `issue` refers to the type of resource we're creating, which in this case is a GitHub issue.
- `create` is the action we want to take, which is to create a new issue.

When you run the `gh issue create` command, you will be prompted for various details about the issue you want to create, such as the issue's title, description, labels, and assignees. Once you enter all the required information, a new issue will be created in your repository.

Here is an example of how you might use `gh issue create`:

```
$ gh issue create --title "Fix bug in login page" --body "The login page is not rendering correctly on mobile" --assignee "octocat" --label "bug"
```

In this example, the command creates a new issue titled "Fix bug in login page" with a description body of "The login page is not rendering correctly on mobile". The issue is assigned to the user "octocat" and given a label of "bug". 

## tldr 
 
> Create GitHub issues on a repository from the command-line.
> More information: <https://cli.github.com/manual/gh_issue_create>.

- Create a new issue against the current repository interactively:

`gh issue create`

- Create a new issue with the `bug` label interactively:

`gh issue create --label "{{bug}}"`

- Create a new issue interactively and assign it to the specified users:

`gh issue create --assignee {{user1,user2,...}}`

- Create a new issue with a title, body and assign it to the current user:

`gh issue create --title "{{title}}" --body "{{body}}" --assignee "{{@me}}"`

- Create a new issue interactively, reading the body text from a file:

`gh issue create --body-file {{path/to/file}}`

- Create a new issue in the default web browser:

`gh issue create --web`

- Display the help:

`gh issue create --help`
