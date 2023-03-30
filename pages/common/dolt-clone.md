# dolt clone 
## chatgpt 
The `dolt clone` command is a command used in the Dolt data-migration system, which is an open-source version control system built for data. 

This command is used to create a copy of an existing Dolt database (repository) from a remote source and creates a local copy of the database that can be accessed and modified. The command is executed by typing `dolt clone [repository]<repo name>` on the command line. 

The `repository` argument specifies the URL of the repository that you want to clone. Once the command is executed, Dolt will create a new directory with the specified `<repo name>` and clone the repository from the specified URL into that directory.

The `dolt clone` command can be used in conjunction with other Dolt commands to allow users to replicate and work with the same datasets across multiple machines, as well as to keep track of changes to the data in a version-controlled environment. 

## tldr 
 
> Clone a repository into a new directory.
> More information: <https://docs.dolthub.com/interfaces/cli#dolt-clone>.

- Clone an existing repository into a specific directory (defaults to the repository name):

`dolt clone {{repository_url}} {{path/to/directory}}`

- Clone an existing repository and add a specific remote (defaults to origin):

`dolt clone --remote {{remote_name}} {{repository_url}}`

- Clone an existing repository only fetching a specific branch (defaults to all branches):

`dolt clone --branch {{branch_name}} {{repository_url}}`

- Clone a repository, using an AWS region (uses the profile's default region if none is provided):

`dolt clone --aws-region {{region_name}} {{repository_url}}`

- Clone a repository, using an AWS credentials file:

`dolt clone --aws-creds-file {{credentials_file}} {{repository_url}}`

- Clone a repository, using an AWS credentials profile (uses the default profile if none is provided):

`dolt clone --aws-creds-profile {{profile_name}} {{repository_url}}`

- Clone a repository, using an AWS credentials type:

`dolt clone --aws-creds-type {{credentials_type}} {{repository_url}}`
