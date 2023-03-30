# git-imerge 
## chatgpt 
`git-imerge` is a command used in Git to interactively merge multiple Git commits into one single commit. It uses an interactive shell to perform this operation, and it offers several options to tailor the merge process according to the specific requirements of the user.

The `git-imerge` command works in three phases:

1. It creates a new commit for each Git commit being merged
2. It interacts with the user to allow them to select which commits should be included in the final commit
3. It generates a new commit that includes all selected commits

Some of the options available with `git-imerge` include:

- `--start [commit]`: This option specifies the starting commit to use for interactive merging.
- `--exclude [commit]`: This option specifies a commit to exclude from the interactive merging process.
- `--into [branch]`: This option specifies the branch to merge the commits into.
- `--no-edit`: This option allows you to skip the interactive commit message editor and use a default commit message.

In summary, `git-imerge` is a powerful tool that can help Git users to combine multiple commits into a single commit, making version control and collaboration more straightforward and efficient. 

## tldr 
 
> Perform a merge or rebase between two Git branches incrementally.
> Conflicts between branches are tracked down to pairs of individual commits, to simplify conflict resolution.
> More information: <https://github.com/mhagger/git-imerge>.

- Start imerge-based rebase (checkout the branch to be rebased, first):

`git imerge rebase {{branch_to_rebase_onto}}`

- Start imerge-based merge (checkout the branch to merge into, first):

`git imerge merge {{branch_to_be_merged}}`

- Show ASCII diagram of in-progress merge or rebase:

`git imerge diagram`

- Continue imerge operation after resolving conflicts (`git add` the conflicted files, first):

`git imerge continue --no-edit`

- Wrap up imerge operation, after all conflicts are resolved:

`git imerge finish`

- Abort imerge operation, and return to the previous branch:

`git-imerge remove && git checkout {{previous_branch}}`
