# git cat-file 
## chatgpt 
The `git cat-file` command is used to view the contents of a Git object. The command takes the SHA-1 id of the object as an argument and returns the contents of that object.

There are several options that can be used with the `git cat-file` command:

- `-t`: This option will print the object type (e.g. blob, tree, commit, tag).
- `-s`: This option will print the object size.
- `-e`: This option will exit with a non-zero status if an object is not found.
- `-p`: This option will pretty-print the contents of the object.

For example, to view the contents of a blob object with SHA-1 id `abc123`, you can use the command:

```
git cat-file -p abc123
```

This will print the contents of the blob object in the terminal. 

## tldr 
 
> Provide content or type and size information for Git repository objects.
> More information: <https://git-scm.com/docs/git-cat-file>.

- Get the [s]ize of the HEAD commit in bytes:

`git cat-file -s HEAD`

- Get the [t]ype (blob, tree, commit, tag) of a given Git object:

`git cat-file -t {{8c442dc3}}`

- Pretty-[p]rint the contents of a given Git object based on its type:

`git cat-file -p {{HEAD~2}}`
