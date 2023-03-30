# git fork 
## chatgpt 
The "git fork" command creates a copy of a Git repository on a remote server, creating a new branch for the user who issued the command. This creates two identical copies, one that belongs to the original repository owner and another that belongs to the user who forked it.

A forked repository allows users to make changes to the codebase without affecting the original repository. Users can push changes to their forked repository, create new branches, and make pull requests to merge their changes back into the original repository.

Forking is commonly used in open-source projects to allow multiple developers to contribute to a single codebase. It also enables developers to work on experimental or customized versions of a project without affecting the mainline codebase.

To fork a repository, a user must have the appropriate permissions to do so. The forked repository is essentially a clone of the original repository, so it contains all the code and commits that the original repository has up to the point of forking.

After forking a repository, a user can continue working on their forked copy, make commits, and push those changes back to their repo, and then create a pull request to merge their changes into the original repository. 

## tldr 
 
> Fork the given GitHub repo. Like `git clone` but forks first.
> Part of `git-extras`.
> More information: <https://github.com/tj/git-extras/blob/master/Commands.md#git-fork>.

- Fork and clone a GitHub repository by its URL:

`git fork {{https://github.com/tldr-pages/tldr}}`

- Fork and clone a GitHub repository by its slug:

`git fork {{tldr-pages/tldr}}`
