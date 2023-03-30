# gh 
## chatgpt 
The command "gh" is a command-line interface tool that provides various git-related functionalities. It is a shorthand for the GitHub CLI tool, which is a command-line interface for GitHub.

The "gh" command can perform various operations such as creating, cloning, and managing repositories, opening pull requests, reviewing code, managing issues and pull requests, running workflows, and many more. It can also integrate with other tools like text editors, terminals, and web browsers.

To use the "gh" command, you must have it installed on your system. Once installed, you can open your terminal and type "gh" followed by the desired command and its options.

For example, to clone a repository, you can use the "gh repo clone <repository-url>" command. Similarly, to create a new repository, you can use the "gh repo create <repository-name>" command. The "gh issue create" command can be used to create a new issue, and the "gh pr create" command can be used to create a new pull request.

The "gh" command also provides help documentation that can be accessed using the "gh help" command. It shows a list of available commands, their brief descriptions, and examples of their usage.

Overall, the "gh" command is a very useful and efficient tool for GitHub users who prefer to work on the command line. It saves time and effort by providing a streamlined way to perform various git-related operations. 

## tldr 
 
> Work seamlessly with GitHub from the command-line.
> Some subcommands such as `gh config` have their own usage documentation.
> More information: <https://cli.github.com/>.

- Clone a GitHub repository locally:

`gh repo clone {{owner}}/{{repository}}`

- Create a new issue:

`gh issue create`

- View and filter the open issues of the current repository:

`gh issue list`

- View an issue in the default web browser:

`gh issue view --web {{issue_number}}`

- Create a pull request:

`gh pr create`

- View a pull request in the default web browser:

`gh pr view --web {{pr_number}}`

- Check out a specific pull request locally:

`gh pr checkout {{pr_number}}`

- Check the status of a repository's pull requests:

`gh pr status`
