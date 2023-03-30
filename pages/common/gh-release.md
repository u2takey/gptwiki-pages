# gh release 
## chatgpt 
`gh release` is a command that is used to manage releases in GitHub. This command helps users to create, view, edit, delete, and publish releases for a repository. 

The syntax for the command is as follows:

```
gh release <command> [flags]
```

Some of the commonly used commands with `gh release` are:

- `create`: This command is used to create a new release for a repository. By default, it creates a draft release, which can be edited before it is published to the public. The command syntax for creating a new release is:
```
gh release create <tag_name> [flags]
```
- `view`: This command is used to view the details of a particular release, such as the release title, description, and assets. The command syntax for viewing a release is:
```
gh release view <tag_name> [flags]
```
- `edit`: This command is used to edit the details of an existing release. The command syntax for editing a release is:
```
gh release edit <tag_name> [flags]
```
- `delete`: This command is used to delete an existing release. The command syntax for deleting a release is:
```
gh release delete <tag_name> [flags]
```
- `publish`: This command is used to publish an existing draft release. Once a release is published, it becomes visible to the public. The command syntax for publishing a release is:
```
gh release publish <tag_name> [flags]
```
Overall, `gh release` is a powerful command that makes it easy for developers to manage releases in GitHub. 

## tldr 
 
> Manage GitHub releases from the command-line.
> More information: <https://cli.github.com/manual/gh_release>.

- List releases in a GitHub repository, limited to 30 items:

`gh release list`

- Display information about a specific release:

`gh release view {{tag}}`

- Create a new release:

`gh release create {{tag}}`

- Delete a specific release:

`gh release delete {{tag}}`

- Download assets from a specific release:

`gh release download {{tag}}`

- Upload assets to a specific release:

`gh release upload {{tag}} {{path/to/file1}} {{path/to/file2}}`
