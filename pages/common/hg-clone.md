# hg clone 
## chatgpt 
The command "hg clone" is used in the Mercurial version control system to create a copy (or clone) of an existing repository. This command creates a new repository that contains a copy of all the files and version history of the original repository.

The syntax of the command is:

hg clone [options] [source] [destination]

Here, [source] is the URL or local path of the repository that you want to clone, and [destination] is the location where you want to create the new clone.

Some common options that can be used with the "hg clone" command are:

- -U: Update to the latest version of the repository after cloning
- -e: Run a specific command or script after clone is complete
- -r: Clone a specific revision of the repository
- -b: Clone a specific branch of the repository

When you run the "hg clone" command, Mercurial creates a new directory with the same name as the repository being cloned, and downloads a copy of all the files and version history into this new directory. This new repository can then be used and modified independently of the original repository. 

## tldr 
 
> Create a copy of an existing repository in a new directory.
> More information: <https://www.mercurial-scm.org/doc/hg.1.html#clone>.

- Clone a repository to a specified directory:

`hg clone {{remote_repository_source}} {{destination_path}}`

- Clone a repository to the head of a specific branch, ignoring later commits:

`hg clone --branch {{branch}} {{remote_repository_source}}`

- Clone a repository with only the `.hg` directory, without checking out files:

`hg clone --noupdate {{remote_repository_source}}`

- Clone a repository to a specific revision, tag or branch, keeping the entire history:

`hg clone --updaterev {{revision}} {{remote_repository_source}}`

- Clone a repository up to a specific revision without any newer history:

`hg clone --rev {{revision}} {{remote_repository_source}}`
