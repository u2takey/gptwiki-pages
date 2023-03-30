# gh pr create 
## chatgpt 
The command "gh pr create" is a command used in the GitHub CLI tool, which is used to create a new pull request for a specific repository.

Here is a breakdown of the command:

- "gh" is the keyword used to call the GitHub CLI tool.
- "pr" stands for "pull request".
- "create" is the command used to create a new pull request.

When you run this command, you will be prompted to choose the repository that you want to create the pull request for. Once you have selected the repository, you will be prompted to enter some additional information such as the title and description of the pull request, the branch you want to merge, and the target branch.

Once you have entered all the required information, the GitHub CLI tool will create the pull request for you and display the URL of the new pull request. This allows you to quickly and easily create new pull requests without having to navigate to the GitHub website. 

## tldr 
 
> Manage GitHub pull requests from the command-line.
> More information: <https://cli.github.com/manual/gh_pr_create>.

- Interactively create a pull request:

`gh pr create`

- Create a pull request, determining the title and description from the commit messages of the current branch:

`gh pr create --fill`

- Create a draft pull request:

`gh pr create --draft`

- Create a pull request specifying the base branch, title, and description:

`gh pr create --base {{base_branch}} --title "{{title}}" --body "{{body}}"`

- Start opening a pull request in the default web browser:

`gh pr create --web`
