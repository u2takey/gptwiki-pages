# scoop bucket 
## chatgpt 
Scoop is a command-line package manager for Windows that allows users to quickly and easily install software packages, tools, and utilities from a command prompt. 

The "scoop bucket" command is used to manage buckets in Scoop. Buckets are repositories or collections of software packages that Scoop can use to install software. When you run "scoop bucket", you will see a list of options you can use with this command. These options include:

- "add": This option is used to add a new bucket to Scoop. You can add a bucket using a URL or a local file path.
- "rm": This option is used to remove an existing bucket from Scoop.
- "list": This option is used to list all the available buckets in Scoop.
- "known": This option is used to show all the known buckets in Scoop, including those that are not currently added to your Scoop installation.
- "cache": This option is used to clear the cache for a specific bucket.

Overall, "scoop bucket" is a useful command for managing software packages and repositories in Scoop, which can help make software installation and management on Windows systems more efficient and streamlined. 

## tldr 
 
> Manage buckets: Git repositories containing files which describe how scoop installs applications.
> If Scoop doesn't know where the bucket is located its repository location must be specified.
> More information: <https://github.com/lukesampson/scoop/wiki/Buckets>.

- List all buckets currently in use:

`scoop bucket list`

- List all known buckets:

`scoop bucket known`

- Add a known bucket by its name:

`scoop bucket add {{name}}`

- Add an unknown bucket by its name and Git repository URL:

`scoop bucket add {{name}} {{https://example.com/repository.git}}`

- Remove a bucket by its name:

`scoop bucket rm {{name}}`
