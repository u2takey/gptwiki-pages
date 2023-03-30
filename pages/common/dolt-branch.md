# dolt branch 
## chatgpt 
The `dolt branch` command is used in the Dolt database system, which is a SQL database system that has Git-like version control built into it. This command is used to perform operations related to branches in Dolt.

When executed without any arguments, the `dolt branch` command will display a list of all branches that exist in the current Dolt repository, along with a marker next to the currently checked out branch.

The command can also be used with argument(s) to perform different operations related to branches. For example, the following are some of the most commonly used arguments with this command:

- `dolt branch <branch-name>`: This will create a new branch with the specified name at the current commit.
- `dolt branch -d <branch-name>`: This will delete the branch with the specified name.
- `dolt branch -m <branch-name> <new-name>`: This will rename the branch with the specified name to a new name.
- `dolt branch -r`: This will display a list of all remote branches in the repository.

Overall, the `dolt branch` command is a powerful tool for managing branches in the Dolt database system. 

## tldr 
 
> Manage Dolt branches.
> More information: <https://github.com/dolthub/dolt>.

- List local branches (current branch is highlighted by `*`):

`dolt branch`

- List all local and remote branches:

`dolt branch --all`

- Create a new branch based on the current branch:

`dolt branch {{branch_name}}`

- Create a new branch with the specified commit as the latest:

`dolt branch {{branch_name}} {{commit}}`

- Rename a branch:

`dolt branch --move {{branch_name1}} {{branch_name2}}`

- Duplicate a branch:

`dolt branch --copy {{branch_name1}} {{branch_name2}}`

- Delete a branch:

`dolt branch --delete {{branch_name}}`

- Display the name of the current branch:

`dolt branch --show-current`
