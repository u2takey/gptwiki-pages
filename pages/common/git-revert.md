# git revert 
## chatgpt 
The "git revert" command in Git is used to create a new commit that undoes the changes made in a previous commit or set of commits. The history of the repository is not rewritten or deleted, but a new commit is created that undoes the changes of the previous commit. This is useful when you want to remove the changes introduced by a commit without removing the commit itself from the Git history.

To use the "git revert" command, you need to specify the commit that you want to undo, either by its hash or by its reference (such as its branch name or tag name).

The complete syntax for "git revert" command is: 

```
git revert <commit>
```

For example, to revert the changes made in the previous commit, you can use:

```
git revert HEAD
```

You can also revert multiple commits at once by specifying their hashes or references:

```
git revert <commit1> <commit2> <commit3>
```

When you run the "git revert" command, Git will open a text editor to allow you to enter a commit message for the new commit. By default, Git pre-fills the message with a description of the changes being reverted, but you can modify it as needed.

Once you save the commit message and close the editor, Git will create a new commit that undoes the changes of the specified commit(s). This new commit will become the new head of the current branch, and the changes will be reflected in your local repository. You can then push this new commit to a remote repository if needed. 

## tldr 
 
> Create new commits which reverse the effect of earlier ones.
> More information: <https://git-scm.com/docs/git-revert>.

- Revert the most recent commit:

`git revert {{HEAD}}`

- Revert the 5th last commit:

`git revert HEAD~{{4}}`

- Revert a specific commit:

`git revert {{0c01a9}}`

- Revert multiple commits:

`git revert {{branch_name~5..branch_name~2}}`

- Don't create new commits, just change the working tree:

`git revert -n {{0c01a9..9a1743}}`
