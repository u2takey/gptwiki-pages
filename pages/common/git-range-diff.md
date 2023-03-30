# git range-diff 
## chatgpt 
The `git range-diff` command is used to compare two commits, giving a summary of the differences between them. Specifically, it shows the difference between the changes in the second commit compared to the first commit, including any changes made to existing lines of code, new lines of code, or deletions.

The basic syntax of the `git range-diff` command is:

```
git range-diff commit1..commit2
```

where `commit1` and `commit2` are the two commits being compared. This can also be shortened to `git range-diff commit1 commit2`.

When run, the command outputs a list of changes between the two commits, including a summary of added, deleted, and modified lines of code. The output is divided into three sections:

1. "Baseline" - the state of the repository before the changes of `commit2` were made
2. "Range" - the changes made by `commit2` in the context of the "Baseline"
3. "Patch" - the actual changes made by `commit2`

Each section includes a list of file names, as well as an overview of the changes made to each file. The changes themselves are displayed as a unified diff, showing the modifications made to individual lines of code.

Overall, `git range-diff` provides a useful overview of the changes made between two commits, making it easier for developers to understand and review changes in their codebase. 

## tldr 
 
> Compare two commit ranges (e.g. two versions of a branch).
> More information: <https://git-scm.com/docs/git-range-diff>.

- Diff the changes of two individual commits:

`git range-diff {{commit_1}}^! {{commit_2}}^!`

- Diff the changes of ours and theirs from their common ancestor, e.g. after an interactive rebase:

`git range-diff {{theirs}}...{{ours}}`

- Diff the changes of two commit ranges, e.g. to check whether conflicts have been resolved appropriately when rebasing commits from `base1` to `base2`:

`git range-diff {{base1}}..{{rev1}} {{base2}}..{{rev2}}`
