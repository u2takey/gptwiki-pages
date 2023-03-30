# git submodule 
## chatgpt 
The `git submodule` command is used in Git to add a reference to a repository inside another repository. This allows you to keep the two repositories separate but linked, so that if changes are made to one repository, they can be easily updated in the other.

Here are the different ways the `git submodule` command can be used:

1. Add a submodule: `git submodule add <repository URL> <directory>`

This command adds a reference to the specified repository inside the current repository. The `<directory>` parameter specifies the name of the directory where the submodule should be added. 

2. Update a submodule: `git submodule update --remote`

This command updates the specified submodule to the latest commit of the branch it is tracking. The `--remote` flag ensures that the update comes from the remote repository.

3. Initialize submodules: `git submodule init`

This command initializes all of the submodules in the repository. It reads the `.gitmodules` file and clones each repository referenced there.

4. List submodules: `git submodule status`

This command displays information about the submodules in the repository, including the branch they are tracking and the current commit they are on.

Overall, the `git submodule` command is a useful tool for managing dependencies and linking related repositories together. 

## tldr 
 
> Inspects, updates and manages submodules.
> More information: <https://git-scm.com/docs/git-submodule>.

- Install a repository's specified submodules:

`git submodule update --init --recursive`

- Add a Git repository as a submodule:

`git submodule add {{repository_url}}`

- Add a Git repository as a submodule at the specified directory:

`git submodule add {{repository_url}} {{path/to/directory}}`

- Update every submodule to its latest commit:

`git submodule foreach git pull`
