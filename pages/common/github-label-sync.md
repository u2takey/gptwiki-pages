# github-label-sync 
## chatgpt 
`github-label-sync` is a command line tool for synchronizing labels across multiple repositories on GitHub. This tool allows users to manage labels in an easy, centralized way, eliminating the need to manually add, remove, or modify labels across different repositories.

The syntax for the `github-label-sync` command is:

```
github-label-sync [--access-token=<TOKEN>] [--endpoint=<ENDPOINT>] [--force] [--dry-run] <SOURCE-REPO> <DEST-REPO> [<DEST-REPO>...]
```

Here, the options are:

- `--access-token=<TOKEN>`: This option allows users to authenticate with GitHub using a personal access token, which is required to access private repositories. Without an access token, only public repositories can be accessed.

- `--endpoint=<ENDPOINT>`: This option sets the GitHub API endpoint to use. By default, this is the main GitHub API at `https://api.github.com/`, but it can be changed to a custom endpoint if necessary.

- `--force`: This option forces the synchronization of all labels, even if they already exist in the destination repositories.

- `--dry-run`: This option simulates the synchronization process without actually modifying any labels.

The arguments are:

- `<SOURCE-REPO>`: This is the name of the source repository to synchronize labels from.

- `<DEST-REPO>`: These are the names of the destination repositories to synchronize labels to. Multiple repository names can be provided, separated by spaces.

When `github-label-sync` is run, it first reads all of the labels from the source repository. Then, for each destination repository, it compares the labels in the source repository to the ones in the destination repository. If a label exists in the source but not in the destination, `github-label-sync` adds the label to the destination repository. If a label exists in the destination but not in the source, `github-label-sync` removes the label from the destination repository. If a label exists in both the source and the destination, the label is updated in the destination repository to match the one in the source. The `--force` option can be used to ensure that all labels are synchronized, even if they already exist in the destination repositories.

Finally, the `--dry-run` option can be used to simulate the synchronization process without actually modifying any labels, allowing users to preview the changes that will be made. 

## tldr 
 
> A command-line interface for synchronizing GitHub labels.
> More information: <https://github.com/Financial-Times/github-label-sync>.

- Synchronize labels using a local `labels.json` file:

`github-label-sync --access-token {{token}} {{repository_name}}`

- Synchronize labels using a specific labels JSON file:

`github-label-sync --access-token {{token}} --labels {{url|path/to/json_file}} {{repository_name}}`

- Perform a dry run instead of actually synchronizing labels:

`github-label-sync --access-token {{token}} --dry-run {{repository_name}}`

- Keep labels that aren't in `labels.json`:

`github-label-sync --access-token {{token}} --allow-added-labels {{repository_name}}`

- Synchronize using the `GITHUB_ACCESS_TOKEN` environment variable:

`github-label-sync {{repository_name}}`
