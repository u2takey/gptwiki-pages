# git rebase 
## chatgpt 
Git rebase is a Git command that allows you to apply the changes made in one branch to another branch. The command takes the commits from one branch, applies them on top of the current branch at the specified point, and creates a new linear branch history.

Here is the syntax for the git rebase command:

```
git rebase [options] [branch]
```

The `[options]` parameter contains different options that you can use with the rebase command. Here are some of the most common ones:

- `-i`: Launches an interactive rebase, which allows you to choose which commits to apply, and how to modify them.
- `--onto [newbase]`: Specifies a new base branch to create the new branch from.
- `-p`: Preserves merge commits when rebasing.

The `[branch]` parameter specifies the branch that you want to apply changes from. By default, Git applies the changes from the current branch to the specified branch.

When you run the `git rebase` command, Git will try to apply the changes from the specified branch onto the current branch. If there are any conflicts, Git will pause the rebase process and prompt you to resolve the conflicts before continuing.

Once the rebase is complete, you will have a new branch with a linear history that contains all the changes from both branches. It's important to note that the original branch will not be modified by the rebase process, and the changes will only be applied to the new branch.

Overall, `git rebase` can be a powerful tool for managing your Git repository's history and organizing your code changes. However, it's important to use it carefully and understand the implications of modifying a branch's history. 

## tldr 
 
> Reapply commits from one branch on top of another branch.
> Commonly used to "move" an entire branch to another base, creating copies of the commits in the new location.
> More information: <https://git-scm.com/docs/git-rebase>.

- Rebase the current branch on top of another specified branch:

`git rebase {{new_base_branch}}`

- Start an interactive rebase, which allows the commits to be reordered, omitted, combined or modified:

`git rebase -i {{target_base_branch_or_commit_hash}}`

- Continue a rebase that was interrupted by a merge failure, after editing conflicting files:

`git rebase --continue`

- Continue a rebase that was paused due to merge conflicts, by skipping the conflicted commit:

`git rebase --skip`

- Abort a rebase in progress (e.g. if it is interrupted by a merge conflict):

`git rebase --abort`

- Move part of the current branch onto a new base, providing the old base to start from:

`git rebase --onto {{new_base}} {{old_base}}`

- Reapply the last 5 commits in-place, stopping to allow them to be reordered, omitted, combined or modified:

`git rebase -i {{HEAD~5}}`

- Auto-resolve any conflicts by favoring the working branch version (`theirs` keyword has reversed meaning in this case):

`git rebase -X theirs {{branch_name}}`
