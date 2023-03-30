# git cherry 
## chatgpt 
The `git cherry` command is used to list the commits that are not yet merged from one branch to another.

The syntax of the command is as follows:

```
git cherry [options] <branch> [<upstream>]
```

Here, the `<branch>` argument is the branch for which you want to see the commits that are not yet merged, and `<upstream>` is the branch which serves as the upstream branch. If `<upstream>` is not specified, it defaults to the upstream branch of the current branch.

Some commonly used options with the `git cherry` command are:

- `-v`: Show the commit messages along with the commit SHA.
- `-n`: Show only the number of commits that are not yet merged.
- `-x`: Show the commit message and the patch introduced by the commit.

When you run the `git cherry` command, it shows the SHA of the commits that are in the `<branch>` but not in the `<upstream>` branch. If a commit already exists in the `<upstream>` branch, it is not shown in the output of the `git cherry` command.

The output of the command may look something like this:

```
+ a5b5d5a5c5a5c5f5d5f5f5c5a5d5a5c5f5a5a5f5 Added feature A
- b4c4d4e4f4b4d4e4f4d4e4c4b4e4d4f4e4c4 Fixed bug B
+ 0c0c1b2a2c2d2b0c1b2a0c2d2b1c0b2a1c Added feature C
```

Here, the `+` sign denotes the commits that are in `<branch>` but not in `<upstream>`, and the `-` sign denotes the commits that are in `<upstream>` but not in `<branch>`. The commit message is also shown along with the commit SHA. 

## tldr 
 
> Find commits that have yet to be applied upstream.
> More information: <https://git-scm.com/docs/git-cherry>.

- Show commits (and their messages) with equivalent commits upstream:

`git cherry -v`

- Specify a different upstream and topic branch:

`git cherry {{origin}} {{topic}}`

- Limit commits to those within a given limit:

`git cherry {{origin}} {{topic}} {{base}}`
