# git stash 
## chatgpt 
The Git stash command is used to temporarily save uncommitted changes in a working directory, allowing the user to switch to a different branch or commit without losing the changes they have made.

Here's how it works:

1. First, navigate to the directory where you have your Git repository.
2. Make some changes to your files in the working directory.
3. Run the command "git stash". This will stash any changes you have made since the last commit.
4. You can now switch to a different branch or commit using "git checkout" without worrying about losing your changes.
5. When you are ready to retrieve your changes, you can run "git stash apply". This will apply the most recent stash and restore your changes to the working directory.
6. If you have multiple stashes, you can specify which one to apply using "git stash apply stash@{n}" where "n" is the number of the stash you want to apply.
7. You can also run "git stash list" to see a list of all stashes you have made, with their corresponding numbers.

Overall, "git stash" is a useful command when you need to temporarily save your changes without committing them, such as when you need to switch branches or work on multiple features at the same time. 

## tldr 
 
> Stash local Git changes in a temporary area.
> More information: <https://git-scm.com/docs/git-stash>.

- Stash current changes, except new (untracked) files:

`git stash push -m {{optional_stash_message}}`

- Stash current changes, including new (untracked) files:

`git stash -u`

- Interactively select parts of changed files for stashing:

`git stash -p`

- List all stashes (shows stash name, related branch and message):

`git stash list`

- Show the changes as a patch between the stash (default is stash@{0}) and the commit back when stash entry was first created:

`git stash show -p {{stash@{0}}}`

- Apply a stash (default is the latest, named stash@{0}):

`git stash apply {{optional_stash_name_or_commit}}`

- Drop or apply a stash (default is stash@{0}) and remove it from the stash list if applying doesn't cause conflicts:

`git stash pop {{optional_stash_name}}`

- Drop all stashes:

`git stash clear`
