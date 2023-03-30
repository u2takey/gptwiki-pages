# git squash 
## chatgpt 
The `git squash` command is used to combine multiple commits into a single commit. This helps to keep the commit history clean and concise, especially when a feature is developed over several commits. The squashed commit will contain the changes made in each individual commit, but they will all be combined into a single commit message with a single commit hash.

Here are the steps to squash commits using the `git squash` command:

1. First, ensure that you are on the branch you want to squash commits from.

2. Use the `git log` command to view the commit history and identify the commits you want to squash. Note down the hash values of these commits.

3. Use the `git rebase -i` command followed by the hash value of the commit before the first commit to be squashed. This will open the interactive rebase window.

4. Change the word "pick" to "squash" or "s" in the commit messages of the commits that need to be squashed.

5. Save and close the rebase file.

6. An editor will open to provide a new commit message, containing the sum of all the squashed commits.

7. Save and close the file to finish the squashing process.

8. Use the `git log` command again to verify that the squashed commit has been created.

It is important to note that you should only squash commits that have not been pushed to a public repository, as it can cause conflicts for other users who have already pulled the commits. 

## tldr 
 
> Squash multiple commits into a single commit.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-squash>.

- Merge all commits from a specific branch into the current branch as a single commit:

`git squash {{source_branch}}`

- Squash all commits starting with a specific commit on the current branch:

`git squash {{commit}}`

- Squash the `n` latest commits and commit with a message:

`git squash HEAD~{{n}} "{{message}}"`

- Squash the `n` latest commits and commit concatenating all individual messages:

`git squash --squash-msg HEAD~{{n}}`
