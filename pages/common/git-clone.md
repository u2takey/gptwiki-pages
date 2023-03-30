# git clone 
## chatgpt 
`git clone` is a command used in Git to create a copy of a remote Git repository onto your local machine. When you clone a Git repository, you are essentially downloading a copy of the repository that contains all of its files and version history to your local computer.

The command syntax for `git clone` is as follows:

```
git clone <repository URL> <local directory>
```

Here:

- `<repository URL>` refers to the URL of the remote Git repository you want to clone. This can be a URL for a repository hosted on GitHub, Bitbucket, GitLab or elsewhere.
- `<local directory>` refers to the name of the directory where you want to save the cloned repository on your local machine.

When you run this command, Git will connect to the remote repository, download the entire history of the repository (including all of its files and folders), and save it to your local machine in the specified directory. The cloned repository is a fully functional Git repository, meaning you will be able to make changes, commit them, and push them back to the original remote repository.

`git clone` is a fundamental command in Git and is often the first command developers run when starting a new project or collaborating with other developers on an existing project. 

## tldr 
 
> Clone an existing repository.
> More information: <https://git-scm.com/docs/git-clone>.

- Clone an existing repository:

`git clone {{remote_repository_location}}`

- Clone an existing repository into a specific directory:

`git clone {{remote_repository_location}} {{path/to/directory}}`

- Clone an existing repository and its submodules:

`git clone --recursive {{remote_repository_location}}`

- Clone a local repository:

`git clone -l {{path/to/local/repository}}`

- Clone quietly:

`git clone -q {{remote_repository_location}}`

- Clone an existing repository only fetching the 10 most recent commits on the default branch (useful to save time):

`git clone --depth {{10}} {{remote_repository_location}}`

- Clone an existing repository only fetching a specific branch:

`git clone --branch {{name}} --single-branch {{remote_repository_location}}`

- Clone an existing repository using a specific SSH command:

`git clone --config core.sshCommand="{{ssh -i path/to/private_ssh_key}}" {{remote_repository_location}}`
