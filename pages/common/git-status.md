# git status 
## chatgpt 
The command "git status" is used in the Git version control system to display the current state of the repository, including changes made to files, untracked files, and the current branch.

When you run "git status", you will see the following information:

1. On branch: This is the name of the current branch you are on.

2. Changes not staged for commit: This section lists files that have been modified since the last commit but have not yet been staged.

3. Changes to be committed: This section lists files that have been added or modified and have been staged, meaning they are ready to be committed.

4. Untracked files: This section lists files that Git is not tracking or that have not been added to the staging area using "git add".

5. Branch is up-to-date with 'origin/master': If your repository is connected to a remote repository, this section will show if your local branch is up-to-date with the remote branch.

Running "git status" regularly is useful to get a quick overview of the state of your repository and to ensure that all changes are tracked and committed. 

## tldr 
 
> Show the changes to files in a Git repository.
> Lists changed, added and deleted files compared to the currently checked-out commit.
> More information: <https://git-scm.com/docs/git-status>.

- Show changed files which are not yet added for commit:

`git status`

- Give output in [s]hort format:

`git status -s`

- Don't show untracked files in the output:

`git status --untracked-files=no`

- Show output in [s]hort format along with [b]ranch info:

`git status -sb`
