# git commit 
## chatgpt 
The `git commit` command is used to record changes to the local repository. When you make changes to files in your working directory, you need to stage them for commit using the `git add` command. Once the changes are staged, you can make a commit with a message describing what changes you made.

The syntax for `git commit` is as follows:

```
git commit -m "commit message"
```

The `-m` option is used to add a message to the commit. The message should be descriptive and should explain what changes you made. It should be in present tense and should not exceed 50 characters in the subject line.

By default, `git commit` will open an editor to allow you to write your commit message. However, using the `-m` option allows you to write the message in the command line itself.

Once you make a commit, the changes are saved to the local repository. You can continue to make further changes and commit them as needed. However, it's important to note that commits should be made in small, cohesive chunks that represent a logical unit of work. This makes it easier to track changes and revert them if necessary. 

## tldr 
 
> Commit files to the repository.
> More information: <https://git-scm.com/docs/git-commit>.

- Commit staged files to the repository with a message:

`git commit -m "{{message}}"`

- Commit staged files with a message read from a file:

`git commit --file {{path/to/commit_message_file}}`

- Auto stage all modified files and commit with a message:

`git commit -a -m "{{message}}"`

- Commit staged files and [S]ign them with the GPG key defined in `~/.gitconfig`:

`git commit -S -m "{{message}}"`

- Update the last commit by adding the currently staged changes, changing the commit's hash:

`git commit --amend`

- Commit only specific (already staged) files:

`git commit {{path/to/file1}} {{path/to/file2}}`

- Create a commit, even if there are no staged files:

`git commit -m "{{message}}" --allow-empty`
