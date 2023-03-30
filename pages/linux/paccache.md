# paccache 
## chatgpt 
The `paccache` command is used in the Arch Linux distribution to manage the package cache. The package cache contains copies of previously installed packages, which can be useful for reinstalling or rolling back packages. The `paccache` command allows users to manage the package cache by removing old packages or freeing up disk space.

Here are some examples of how to use `paccache`:

1. To display a list of packages in the cache:
```
paccache -l
```
This will display a list of all packages stored in the cache.

2. To remove old packages from the cache:
```
paccache -r
```
This will remove any packages in the cache that are not currently installed on the system.

3. To remove all packages in the cache:
```
paccache -rk0
```
This will remove all packages from the cache.

4. To free up disk space by removing all packages except the most recent two:
```
paccache -rk2
```
This will remove all packages from the cache except the two most recent versions of each package.

In summary, `paccache` is a powerful command that can help users manage the package cache on their Arch Linux system. It can be used to remove old packages, free up disk space, and display information about the packages stored in the cache. 

## tldr 
 
> A pacman cache cleaning utility.
> More information: <https://manned.org/paccache>.

- Remove all but the 3 most recent package versions from the pacman cache:

`paccache -r`

- Set the number of package versions to keep:

`paccache -rk {{num_versions}}`

- Perform a dry-run and show the number of candidate packages for deletion:

`paccache -d`

- Move candidate packages to a directory instead of deleting them:

`paccache -m {{path/to/directory}}`
