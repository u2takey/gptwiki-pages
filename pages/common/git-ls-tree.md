# git ls-tree 
## chatgpt 
The "git ls-tree" command is used to display the contents of a Git tree object. A tree object is a hierarchical structure in Git that contains references to individual files as well as additional tree objects. The tree object represents a directory in a Git repository.

The "ls-tree" command takes one or more arguments. The first argument is the Git reference to the tree object you want to display. This reference can be a branch, a tag or a commit SHA-1 hash. The second argument is the path within the tree object that you want to display. If no path is specified, the entire tree object is displayed.

When executed, "git ls-tree" returns a list of the files and directories contained within the specified tree object. For each file or directory, the command displays its permissions, object type (tree or blob), SHA-1 hash, and its filename.

Overall, "git ls-tree" is useful for inspecting the contents of a tree object in a Git repository, especially when you need to locate a specific file or directory within a particular branch or commit. 

## tldr 
 
> List the contents of a tree object.
> More information: <https://git-scm.com/docs/git-ls-tree>.

- List the contents of the tree on a branch:

`git ls-tree {{branch_name}}`

- List the contents of the tree on a commit, recursing into subtrees:

`git ls-tree -r {{commit_hash}}`

- List only the filenames of the tree on a commit:

`git ls-tree --name-only {{commit_hash}}`
