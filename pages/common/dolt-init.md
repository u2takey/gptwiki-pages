# dolt init 
## chatgpt 
The `dolt init` command initializes a new Dolt repository within the current directory.

When you run this command, Dolt creates all the necessary directories and files, including a `.dolt` directory that holds the repository metadata, a `dolt` binary file that is used to interact with the repository, and a `README.md` file that provides basic information about the repository.

Note that running `dolt init` in an existing directory will overwrite any existing Dolt files and directories, so be careful if you have pre-existing Dolt repositories in the current directory.

After running `dolt init`, you can begin adding data to your repository using Dolt's various commands, such as `dolt add`, `dolt commit`, and `dolt push`. 

## tldr 
 
> Create an empty Dolt data repository.
> More information: <https://docs.dolthub.com/cli-reference/cli#dolt-init>.

- Initialize a new Dolt data repository in the current directory:

`dolt init`

- Initialize a new Dolt data repository creating a commit with the specified metadata:

`dolt init --name "{{name}}" --email "{{email}}" --date "{{2021-12-31T00:00:00}}" -b "{{branch_name}}"`
