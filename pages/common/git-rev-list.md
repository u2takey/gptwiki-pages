# git rev-list 
## chatgpt 
`git rev-list` is a Git command used to list out the commit objects in reverse chronological order. It is a shorthand for `git log --no-walk`, which lists the SHA1 hash of each commit in the current branch.

The `git rev-list` command supports a range of options that can be used to narrow down the output. 

Some common options include:

- `--max-count=<number>`: Limits the number of commits to display
- `--first-parent`: Only follows the first parent commit when merging
- `--ancestry-path <commit>..<commit>`: Prints the commits that are ancestors of the second commit but not the first commit
- `--date=<format>`: Changes the date format used when displaying the commit logs

Example usage:

To list all the commits in the current branch:

```
$ git rev-list HEAD
```

To list the last five commits in the current branch:

```
$ git rev-list HEAD --max-count=5
```

To list the first parent commits for each merge commit:

```
$ git rev-list --first-parent --merges HEAD
```

Overall, `git rev-list` is a useful command for exploring a Git repository's commit history and finding specific commits to work with. 

## tldr 
 
> List revisions (commits) in reverse chronological order.
> More information: <https://git-scm.com/docs/git-rev-list>.

- List all commits on the current branch:

`git rev-list {{HEAD}}`

- Print the latest commit that changed (add/edit/remove) a specific file on the current branch:

`git rev-list -n 1 HEAD -- {{path/to/file}}`

- List commits more recent than a specific date, on a specific branch:

`git rev-list --since={{'2019-12-01 00:00:00'}} {{branch_name}}`

- List all merge commits on a specific commit:

`git rev-list --merges {{commit}}`

- Print the number of commits since a specific tag:

`git rev-list {{tag_name}}..HEAD --count`
