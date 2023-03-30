# hg push 
## chatgpt 
"hg push" is a command used in Mercurial, a popular version control system, to upload the changes made in a local repository to a remote repository. 

When executed, "hg push" command checks the default branch to determine the destination of the push operation. If a remote repository is specified, the local changes and revisions are pushed to that repository. If no remote repositories are specified, Mercurial looks for a default remote repository, typically the one from which the repository was cloned. 

Before you can push changes, it is important to ensure that your local repository is up-to-date, and you have committed all your changes to the local repository. It is also essential to ensure that the changes you want to push do not conflict with changes that have been made in the remote repository since your last pull operation. If there are any conflicts, Mercurial will prompt you to resolve them first.

Overall, "hg push" is a very useful command for collaborating on projects and sharing changes with colleagues in a team environment. 

## tldr 
 
> Push changes from the local repository to a specified destination.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#push>.

- Push changes to the "default" remote path:

`hg push`

- Push changes to a specified remote repository:

`hg push {{path/to/destination_repository}}`

- Push a new branch if it does not exist (disabled by default):

`hg push --new-branch`

- Specify a specific revision changeset to push:

`hg push --rev {{revision}}`

- Specify a specific branch to push:

`hg push --branch {{branch}}`

- Specify a specific bookmark to push:

`hg push --bookmark {{bookmark}}`
