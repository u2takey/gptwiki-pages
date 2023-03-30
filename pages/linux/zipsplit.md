# zipsplit 
## chatgpt 
The `zipsplit` command is a Linux/Unix command used for splitting large Zip files into smaller zip archives. The basic syntax used for this command is:

`zipsplit [options] archive.zip [size]`

Here, `archive.zip` refers to the name of the zip file you want to split, and `[size]` refers to the size of the new zip files you want to create. You can specify the size in bytes (B), kilobytes (K), megabytes (M), or gigabytes (G). If you do not specify a size, zipsplit will create as many files as necessary to store the archive.

The available options for this command are as follows:

- `-n`: Specifies the number of pieces to split the archive into. This option can't be used along with the `[size]` parameter.
- `-r`: Renames the original archive to filename.z##
- `-t`: Tests the archive after splitting.
- `-v`: Verbose mode. This will print out some helpful information while the command is running.
- `-h`: Displays the help message for the `zipsplit` command.

For example, to split a zip file named `myarchive.zip` into smaller files of 50 MB each, use the following command:

`zipsplit -n 10 myarchive.zip 50M`

This command will split the `myarchive.zip` file into 10 zip files of 50 MB each.

Note that the `zipsplit` command only splits the Zip file into separate files, and it does not compress the files. If you want to compress the files, you can use the `zip` command. 

## tldr 
 
> Read a zipfile and split it into smaller zipfiles.
> More information: <https://manned.org/zipsplit>.

- Split zipfile into pieces that are no larger than a particular size [n]:

`zipsplit -n {{size}} {{path/to/archive.zip}}`

- [p]ause between the creation of each split zipfile:

`zipsplit -p -n {{size}} {{path/to/archive.zip}}`

- Output the split zipfiles into the `archive` directory:

`zipsplit -b {{archive}} -n {{size}} {{path/to/archive.zip}}`
