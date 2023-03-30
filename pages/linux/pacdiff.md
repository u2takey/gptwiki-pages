# pacdiff 
## chatgpt 
`pacdiff` is a command that is used in Arch Linux and its derivatives to manage and compare the differences between configuration files that have changed after installing a package update.

When a package is updated, its configuration files may undergo changes. These changes may be significant or trivial, but in either case, it is important to be able to identify and manage them properly.

The pacdiff command comes in handy in such situations. It detects a package update that contains modified configuration files and produces a list of the files that have changed. It then prompts the user to compare the old and new versions of each of these files.

The command lists the name of each file that has been modified and for each file, it provides the option to compare the old and new versions side by side, ignore the changes, or merge the differences manually.

By default, pacdiff uses the `vimdiff` editor to compare files, but you can change this by setting the `PACDIFF_EDITOR` variable to your preferred text editor.

Overall, pacdiff is a useful tool for keeping track of package updates and managing configuration file changes properly. 

## tldr 
 
> Maintenance utility for `.pacorig`, `.pacnew` and `.pacsave` files created by `pacman`.
> More information: <https://man.archlinux.org/man/pacdiff>.

- Review files that need maintenance in interactive mode:

`pacdiff`

- Use sudo and sudoedit to remove and merge files:

`pacdiff --sudo`

- Review files needing maintenance, creating `.bak`ups of the original if you `(O)verwrite`:

`pacdiff --sudo --backup`

- Use a specific editor to view and merge configuration files (default is `vim -d`):

`DIFFPROG={{editor}} pacdiff`

- Scan for configuration files with `locate` instead of using pacman database:

`pacdiff --locate`

- Display help:

`pacdiff --help`
