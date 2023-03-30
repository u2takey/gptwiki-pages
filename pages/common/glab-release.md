# glab release 
## chatgpt 
The `glab release` command is a GitLab CLI command used to create, list, update or delete releases. The command allows users to manage git repositories and releases from the command line.

Here's an overview of some of the subcommands and options available with `glab release`:

- `glab release create` - Creates a new release for the repository. This command requires specifying the release name, target commit or tag, and optionally a description and release notes.
- `glab release list` - Lists all existing releases for the repository.
- `glab release show` - Shows details of a specific release. This command requires specifying the release name or tag.
- `glab release edit` - Edits an existing release. This command requires specifying the release name or tag, and optionally a new release name, target commit or tag, description, and release notes.
- `glab release delete` - Deletes a release. This command requires specifying the release name or tag.

Overall, `glab release` is a useful command for managing releases directly from the command line, without the need to navigate through the GitLab web interface. 

## tldr 
 
> Manage GitLab releases from the command-line.
> More information: <https://glab.readthedocs.io/en/latest/release>.

- List releases in a Gitlab repository, limited to 30 items:

`glab release list`

- Display information about a specific release:

`glab release view {{tag}}`

- Create a new release:

`glab release create {{tag}}`

- Delete a specific release:

`glab release delete {{tag}}`

- Download assets from a specific release:

`glab release download {{tag}}`

- Upload assets to a specific release:

`glab release upload {{tag}} {{path/to/file1}} {{path/to/file2}}`
