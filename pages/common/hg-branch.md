# hg branch 
## chatgpt 
The "hg branch" command is used in the Mercurial version control system for creating and switching between named branches. 

A branch is a separate line of development that diverges from the main line of development. This can be useful when you need to work on different features or bug fixes simultaneously without interfering with each other.

The "hg branch" command can be used in various ways:

1. To create a new branch, type "hg branch [branchname]". This will create a new branch with the specified name and switch to it. For example, "hg branch mynewfeature" will create a new branch called "mynewfeature" and switch to it.

2. To switch to an existing branch, type "hg branch [branchname]". This will switch to the specified branch. For example, "hg branch mynewfeature" will switch to the "mynewfeature" branch.

3. To list all branches, type "hg branches". This will display a list of all existing branches.

4. To close a branch, type "hg commit --close-branch". This will close the current branch and mark it as inactive.

Overall, the "hg branch" command is a useful tool for managing multiple lines of development in a Mercurial repository. 

## tldr 
 
> Create or show a branch name.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#branch>.

- Show the name of the currently active branch:

`hg branch`

- Create a new branch for the next commit:

`hg branch {{branch_name}}`
