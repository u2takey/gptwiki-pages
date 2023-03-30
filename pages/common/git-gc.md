# git gc 
## chatgpt 
The `git gc` command is used to perform some maintenance tasks of the Git repository. GC stands for "Garbage Collection," which refers to the process of cleaning up unnecessary or unreachable data from the repository's history. Here are the details of this command:

1. Garbage collection: When you create, modify, or delete files in a Git repository, it creates a new set of commits, branches, and tags. These commits, branches, and tags are stored as "loose objects" in the repository. Over time, this can lead to a large number of loose objects that are no longer needed. The `git gc` command is used to perform garbage collection, which removes these loose objects and frees up disk space.

2. Object compression: When you run the `git gc` command, it will also compress the objects in the repository. This reduces the size of the repository on disk, which can improve performance.

3. Repository optimization: Git uses various algorithms to optimize performance, such as delta compression, which stores only the differences between files instead of the whole file. When you run `git gc`, it will also optimize the repository using these algorithms.

4. Pruning reflog: Git keeps track of references to each commit, which is stored in the "reflog." Over time, this can grow large and take up disk space. `git gc` also prunes the reflog, which removes unnecessary entries and frees up disk space.

Overall, the `git gc` command is used to keep the Git repository performant and optimized. You should run this command periodically to keep your repository in good shape. 

## tldr 
 
> Optimise the local repository by cleaning unnecessary files.
> More information: <https://git-scm.com/docs/git-gc>.

- Optimise the repository:

`git gc`

- Aggressively optimise, takes more time:

`git gc --aggressive`

- Do not prune loose objects (prunes by default):

`git gc --no-prune`

- Suppress all output:

`git gc --quiet`

- View full usage:

`git gc --help`
