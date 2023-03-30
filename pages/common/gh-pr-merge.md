# gh pr merge 
## chatgpt 
The command `gh pr merge` is used to merge a pull request on GitHub from the command line interface using the GitHub CLI tool. 

Here's a breakdown of the command: 

- `gh` refers to the GitHub CLI tool
- `pr` is a shorthand for "pull request" 
- `merge` is the action we want to perform on the pull request 

When you run this command, you'll be prompted to select the pull request you want to merge by its number or by specifying a search term. Once you've selected the right pull request, you'll be prompted to confirm that you want to merge it. 

Here are some additional options you can use with the `gh pr merge` command: 
- `--add-draft` will merge draft pull requests 
- `--merge` specifies the merge method (default is "merge" but you can also use "squash" or "rebase") 
- `--delete-branch` will delete the branch after it has been merged 

Overall, the `gh pr merge` command is a convenient way to merge pull requests from the command line without having to navigate to the GitHub website. 

## tldr 
 
> Merge GitHub pull requests.
> More information: <https://cli.github.com/manual/gh_pr_merge>.

- Merge the pull request associated with the current branch interactively:

`gh pr merge`

- Merge the specified pull request, interactively:

`gh pr merge {{pr_number}}`

- Merge the pull request, removing the branch on both the local and the remote:

`gh pr merge --delete-branch`

- Merge the current pull request with the specified merge strategy:

`gh pr merge --{{merge|squash|rebase}}`

- Merge the current pull request with the specified merge strategy and commit message:

`gh pr merge --{{merge|squash|rebase}} --subject {{commit_message}}`

- Squash the current pull request into one commit with the message body and merge:

`gh pr merge --squash --body="{{commit_message_body}}"`

- Display help:

`gh pr merge --help`
