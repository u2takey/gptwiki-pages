# git format-patch 
## chatgpt 
The `git format-patch` command is used to create patches for one or more Git commits. Here's a breakdown of its options and usage:

Usage:

```
git format-patch [<options>] <commit-range>
```

Options:

- `--stdout`: Sends the output to the console instead of creating a file.
- `--numbered`: Adds a number to the start of each patch file.
- `--no-numbered`: Prevents the addition of a number to the start of each patch file.
- `--thread`: Threads multiple patch files.
- `--no-thread`: Store each patch file in its own thread.
- `--signoff`: Adds a sign-off message to the end of each patch file.
- `--notes[=<ref>]`: Appends notes from the specified note reference to patches.
- `--mbox`: Outputs the patches in mbox format.
- `--ignore-if-in-upstream`: Omits patches which are already present in upstream.

Commit Range:

`<commit-range>` is the range of commits to create patches for. It can be a commit SHA, a branch name or a range of commits using the `..` syntax.

The `git format-patch` command creates one file for each patch, which contains the changes made in the specified commit range. The patch files can be emailed or shared with others to apply the changes on their local Git repository. The files are named according to the commit message and include the commit ID and subject.

The `git format-patch` command is useful when working with other developers and teams, allowing changes to be reviewed and merged easily. 

## tldr 
 
> Prepare .patch files. Useful when emailing commits elsewhere.
> See also `git am`, which can apply generated .patch files.
> More information: <https://git-scm.com/docs/git-format-patch>.

- Create an auto-named `.patch` file for all the unpushed commits:

`git format-patch {{origin}}`

- Write a `.patch` file for all the commits between 2 revisions to `stdout`:

`git format-patch {{revision_1}}..{{revision_2}}`

- Write a `.patch` file for the 3 latest commits:

`git format-patch -{{3}}`
