# standard-version 
## chatgpt 
`standard-version` is a command used in software development to automate the process of versioning and changelog creation. 

The command reads the Git commit messages since the last tagged release, determines the next version number according to the Semantic Versioning specification, creates a Git tag for the new version, and generates a changelog based on the commit messages.

The command also provides options to customize the changelog generation, such as specifying a different commit message format or using custom sections in the changelog.

By using `standard-version`, developers can easily version their software and keep track of changes made between each release, making it easier for users to understand the changes and decide whether to update their software to the newest version. 

## tldr 
 
> Automate versioning and changelog generation, with SemVer and Conventional Commits.
> More information: <https://github.com/conventional-changelog/standard-version>.

- Update the changelog file and tag a release:

`standard-version`

- Tag a release without bumping the version:

`standard-version --first-release`

- Update the changelog and tag an alpha release:

`standard-version --prerelease alpha`

- Update the changelog and tag a specific release type:

`standard-version --release-as {{major|minor|patch}}`

- Tag a release, preventing hooks from being verified during the commit step:

`standard-version --no-verify`

- Tag a release committing all staged changes, not just files affected by `standard-version`:

`standard-version --commit-all`

- Update a specific changelog file and tag a release:

`standard-version --infile {{path/to/file.md}}`

- Display the release that would be performed without performing them:

`standard-version --dry-run`
