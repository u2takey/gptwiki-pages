# git switch 
## chatgpt 
The git switch command allows you to switch between branches or create new ones in your Git repository.

Syntax: `git switch [options] <branch-name>`

The options include:

- `-c`, `--create`: Creates a new branch and switches to it.
- `-d`, `--detach`: Detaches the HEAD from a branch and switches to a specific commit.
- `-l`, `--list`: Lists all local branches.
- `-r`, `--remote`: Allows you to switch to a remote branch.

Examples:

1. To switch to an existing branch: 

```
$ git switch branch-name
```

2. To create a new branch and switch to it:

```
$ git switch -c new-branch
```

3. To list all local branches:

```
$ git switch -l
```

4. To switch to a remote branch:

```
$ git switch -r origin/remote-branch
``` 

## tldr 
 
> Switch between Git branches. Requires Git version 2.23+.
> See also `git checkout`.
> More information: <https://git-scm.com/docs/git-switch>.

- Switch to an existing branch:

`git switch {{branch_name}}`

- Create a new branch and switch to it:

`git switch --create {{branch_name}}`

- Create a new branch based on an existing commit and switch to it:

`git switch --create {{branch_name}} {{commit}}`

- Switch to the previous branch:

`git switch -`

- Switch to a branch and update all submodules to match:

`git switch --recurse-submodules {{branch_name}}`

- Switch to a branch and automatically merge the current branch and any uncommitted changes into it:

`git switch --merge {{branch_name}}`
