# gh pr 
## chatgpt 
The `gh pr` command is a GitHub CLI command used to manage pull requests in a repository. It allows you to view, create, merge, and close pull requests from the command line interface.

Some common use cases of the `gh pr` command are:

- `gh pr view`: Allows you to view the pull request details like status, description, comments, etc.
- `gh pr checkout`: Creates a local branch and checks out a pull request that has not been merged yet.
- `gh pr merge`: Merges the pull request into the main branch of the repository.
- `gh pr create`: Creates a new pull request from the current branch to the main branch in the repository.
- `gh pr list`: Lists all the pull requests in the repository.

To use the `gh pr` command, you need to have the GitHub command-line interface installed on your system along with an authenticated GitHub account. Once you have installed the CLI, you can use the `gh pr` command by typing it into your terminal followed by the specific subcommand and its arguments to perform various actions related to pull requests. 

## tldr 
 
> Manage GitHub pull requests from the command-line.
> Some subcommands such as `gh pr create` have their own usage documentation.
> More information: <https://cli.github.com/manual/gh_pr>.

- Create a pull request:

`gh pr create`

- Check out a specific pull request locally:

`gh pr checkout {{pr_number}}`

- View the changes made in the pull request for the current branch:

`gh pr diff`

- Approve the pull request for the current branch:

`gh pr review --approve`

- Merge the pull request associated with the current branch interactively:

`gh pr merge`

- Edit a pull request interactively:

`gh pr edit`

- Edit the base branch of a pull request:

`gh pr edit --base {{branch_name}}`

- Check the status of the current repository's pull requests:

`gh pr status`
