# git 
## chatgpt 
Git is a distributed version control system used to manage source code and track changes made over time. It was created by Linus Torvalds in 2005 as a way to manage the Linux kernel source code. Git is open source software and is free to use. Here are some common Git commands and what they do:

1. `git init` - Initializes a new repository in the current directory.

2. `git clone` - Creates a copy of an existing repository.

3. `git add` - Adds changes made to files to the staging area to be committed.

4. `git commit` - Saves changes made to files in the repository.

5. `git push` - Uploads local repository commits to a remote repository.

6. `git pull` - Downloads the latest commits from a remote repository.

7. `git log` - Displays a list of previous commits made in the repository.

8. `git branch` - Creates, lists, and deletes branches within the repository.

9. `git merge` - Combines changes made in one branch into another branch.

10. `git status` - Displays the current status of files in the repository.

These commands are just a few basic examples of what Git can do. Git is a powerful tool that can be used to manage and collaborate on projects of all sizes. 

## tldr 
 
> Distributed version control system.
> Some subcommands such as `commit`, `add`, `branch`, `checkout`, `push`, etc. have their own usage documentation, accessible via `tldr git subcommand`.
> More information: <https://git-scm.com/>.

- Check the Git version:

`git --version`

- Show general help:

`git --help`

- Show help on a Git subcommand (like `clone`, `add`, `push`, `log`, etc.):

`git help {{subcommand}}`

- Execute a Git subcommand:

`git {{subcommand}}`

- Execute a Git subcommand on a custom repository root path:

`git -C {{path/to/repo}} {{subcommand}}`

- Execute a Git subcommand with a given configuration set:

`git -c '{{config.key}}={{value}}' {{subcommand}}`
