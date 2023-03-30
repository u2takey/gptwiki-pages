# git show-ref 
## chatgpt 
The `git show-ref` command is a Git command that helps to display the hash values of references or refs in a Git repository. A reference or ref is a mechanism that allows Git to keep track of all the different versions of files and directories in a repository.

When used without any arguments, the `git show-ref` command displays the hash values of all the references in the repository. The command helps to show the current hash values of each branch, tag, or any other reference present in the Git repository.

Here are some useful examples of `git show-ref` command:

1. `git show-ref`: Displays a list of all references with their hash values present in the Git repository.
2. `git show-ref --heads`: Displays a list of all branch references with their hash values present in the Git repository.
3. `git show-ref --tags`: Displays a list of all tag references with their hash values present in the Git repository.
4. `git show-ref <reference>`: Displays the hash value of a specific reference in the Git repository.

In summary, `git show-ref` is a powerful command-line tool that enables developers to track and manage references in a Git repository. The command helps to display detailed information about a specific branch, tag or reference hash values, which can be useful in debugging or troubleshooting issues in the project. 

## tldr 
 
> Git command for listing references.
> More information: <https://git-scm.com/docs/git-show-ref>.

- Show all refs in the repository:

`git show-ref`

- Show only heads references:

`git show-ref --heads`

- Show only tags references:

`git show-ref --tags`

- Verify that a given reference exists:

`git show-ref --verify {{path/to/ref}}`
