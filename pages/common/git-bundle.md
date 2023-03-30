# git bundle 
## chatgpt 
The "git bundle" command in Git is used to create a standalone Git repository, which can be easily shared with others. It allows you to bundle up your Git repository and all of its objects and references into a single file, which can be transferred between repositories, or over a network using various transport protocols.

When you run the "git bundle" command, it creates a binary file (with a ".bundle" extension) that contains all the objects in your Git repository. This file also contains references to all the branches, tags, and commits within your repository at the time of bundling.

The "git bundle" command has a few important options:

- Create: This option specifies that you want to create a bundle file.
- Verify: This option verifies that the specified bundle file is valid and usable as a Git repository.
- List-heads: This option lists all the heads (branch tips) in the bundle.
- Unbundle: This option extracts a Git repository from the specified bundle file.

Overall, the "git bundle" command is very useful for sharing Git repositories without using a centralized server, and it is particularly helpful when you need to transfer repositories to environments without internet connectivity (or via a low-bandwidth connection). 

## tldr 
 
> Package objects and references into an archive.
> More information: <https://git-scm.com/docs/git-bundle>.

- Create a bundle file that contains all objects and references of a specific branch:

`git bundle create {{path/to/file.bundle}} {{branch_name}}`

- Create a bundle file of all branches:

`git bundle create {{path/to/file.bundle}} --all`

- Create a bundle file of the last 5 commits of the current branch:

`git bundle create {{path/to/file.bundle}} -{{5}} {{HEAD}}`

- Create a bundle file of the latest 7 days:

`git bundle create {{path/to/file.bundle}} --since={{7.days}} {{HEAD}}`

- Verify that a bundle file is valid and can be applied to the current repository:

`git bundle verify {{path/to/file.bundle}}`

- Print to the standard output the list of references contained in a bundle:

`git bundle unbundle {{path/to/file.bundle}}`

- Unbundle a specific branch from a bundle file into the current repository:

`git pull {{path/to/file.bundle}} {{branch_name}}`
