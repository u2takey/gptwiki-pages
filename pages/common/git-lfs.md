# git lfs 
## chatgpt 
`git lfs` is a Git extension that enables the use of large file storage (LFS) for version control. 

Large files (such as audio, video or images) can be a problem when storing them in a Git repository because they can make the repository size very large and slow down many Git operations. Git LFS works by replacing large files with a small placeholder file. The actual large file is then stored on a remote LFS server and can be downloaded on-demand when needed.

The `git lfs` command is used to interact with Git LFS. Some common `git lfs` commands are:

- `git lfs track`: specifies which files should be handled by LFS
- `git lfs pull`: downloads all files tracked by LFS that are not currently on the local machine
- `git lfs push`: uploads all changes to large files tracked by LFS
- `git lfs status`: shows the status of LFS files in the repository
- `git lfs logs`: shows the LFS server logs

Git LFS is useful for teams that work with large files, such as multimedia files, game assets, or CAD files. With Git LFS, the repository size remains manageable and Git operations remain fast, even with large files. 

## tldr 
 
> Work with large files in Git repositories.
> More information: <https://git-lfs.github.com>.

- Initialize Git LFS:

`git lfs install`

- Track files that match a glob:

`git lfs track '{{*.bin}}'`

- Change the Git LFS endpoint URL (useful if the LFS server is separate from the Git server):

`git config -f .lfsconfig lfs.url {{lfs_endpoint_url}}`

- List tracked patterns:

`git lfs track`

- List tracked files that have been committed:

`git lfs ls-files`

- Push all Git LFS objects to the remote server (useful if errors are encountered):

`git lfs push --all {{remote_name}} {{branch_name}}`

- Fetch all Git LFS objects:

`git lfs fetch`

- Checkout all Git LFS objects:

`git lfs checkout`
