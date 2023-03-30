# stow 
## chatgpt 
Stow is a command-line utility used for managing the installation and management of multiple versions of software, configurations, and files in a single directory hierarchy. The stow command is used to create, remove, and manage symbolic links between the files or directories and the stow directory tree.

The command syntax for stow is:

```sh
stow [options] [target_directory]
```

where 

- `options`: specifies any additional options to be used with the stow command
- `target_directory`: specifies the directory where stow should install the files or directories

Some of the most common options used with the stow command are:

- `-d`: specifies the parent directory of the stow directory tree
- `-t`: specifies the directory where the symbolic links should be created
- `-v`: enables verbose mode to display detailed output
- `-R`: reverts any previously applied stow actions

Here's an example of how the stow command can be used:

1. Create a directory called "software" for managing installed software versions.

```sh
mkdir software
```

2. Install a software version in the "software" directory using `wget` and `tar` commands.

```sh
wget http://example.com/software.tar.gz
tar -zxvf software.tar.gz
```

3. Use the stow command to manage the installed software.

```sh
stow -d . -t /usr/local/bin software
```

This will create symbolic links to the software version's executable files in the `/usr/local/bin` directory, allowing the software to be used system-wide.

Overall, the stow command is a helpful tool for efficiently managing multiple versions of software, configurations, and files in one place. 

## tldr 
 
> Symlink manager.
> Often used to manage dotfiles.
> More information: <https://www.gnu.org/software/stow>.

- Symlink all files recursively to a given directory:

`stow --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}`

- Delete symlinks recursively from a given directory:

`stow --delete --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}`

- Simulate to see what the result would be like:

`stow --simulate --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}`

- Delete and resymlink:

`stow --restow --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}`

- Exclude files matching a regular expression:

`stow --ignore={{regular_expression}} --target={{path/to/target_directory}} {{file1 directory1 file2 directory2}}`
