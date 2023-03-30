# git worktree 
## chatgpt 
The `git worktree` command is used in Git to create and manage multiple working trees from the same repository. A working tree is a directory within a Git repository that contains a copy of the repository's files, so that users can edit, compile, and test code without altering the original repository.

The `git worktree` command has several sub-commands that enable users to create, list, and delete working trees. Here are some of the most common sub-commands:

- `add`: This command creates a new working tree within the repository. For example, you could use `git worktree add /path/to/new/directory` to create a new working tree in the `/path/to/new/directory` directory.

- `list`: This command lists all the working trees that have been created for the repository. You can use `git worktree list` to see information about the working trees, such as their paths and the branches they are attached to.

- `remove`: This command deletes a working tree that is no longer needed. For example, you could use `git worktree remove /path/to/old/directory` to remove a working tree in the `/path/to/old/directory` directory.

When you create a new working tree with `git worktree add`, it is linked to the main repository in a "detached HEAD" state. This means that changes made in the new working tree do not affect the other working trees or the main repository until they are committed and merged back into the repository.

Overall, `git worktree` is a powerful tool for Git users who need to work on multiple branches or versions of a repository simultaneously, without the risk of conflicting changes or losing work. 

## tldr 
 
> Manage multiple working trees attached to the same repository.
> More information: <https://git-scm.com/docs/git-worktree>.

- Create a new directory with the specified branch checked out into it:

`git worktree add {{path/to/directory}} {{branch}}`

- Create a new directory with a new branch checked out into it:

`git worktree add {{path/to/directory}} -b {{new_branch}}`

- List all the working directories attached to this repository:

`git worktree list`

- Remove a worktree (after deleting worktree directory):

`git worktree prune`
