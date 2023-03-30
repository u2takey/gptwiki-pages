# git apply 
## chatgpt 
The git apply command is used to apply a patch to a repository. A patch is a file containing a set of changes that need to be applied to a specific file.

The syntax for the git apply command is as follows:

```
git apply [options] <patch file>
```

Here, the options are additional arguments that can be used with the command, and the patch file is the file that contains the changes to be applied.

Some common options for the git apply command include:

- `--check`: This option checks whether the patch can be applied cleanly without actually applying it.
- `--index`: This option applies the patch directly to the repository's index instead of the working directory.
- `--reject`: This option creates a `.rej` file for each hunk that cannot be applied to the repository.

When you run the git apply command, Git reads the patch file and applies the changes to the appropriate file or files in the repository. If there are any conflicts with existing changes in the repository, Git will prompt you to resolve them before proceeding.

Overall, the git apply command is a useful tool for selectively applying changes to a repository, especially when working with patches or other changesets. 

## tldr 
 
> Apply a patch to files and/or to the index.
> More information: <https://git-scm.com/docs/git-apply>.

- Print messages about the patched files:

`git apply --verbose {{path/to/file}}`

- Apply and add the patched files to the index:

`git apply --index {{path/to/file}}`

- Apply a remote patch file:

`curl {{https://example.com/file.patch}} | git apply`

- Output diffstat for the input and apply the patch:

`git apply --stat --apply {{path/to/file}}`

- Apply the patch in reverse:

`git apply --reverse {{path/to/file}}`

- Store the patch result in the index without modifying the working tree:

`git apply --cache {{path/to/file}}`
