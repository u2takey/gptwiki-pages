# pax 
## chatgpt 
The "pax" command is a command-line utility for creating, extracting, and modifying archive files in various formats. Pax stands for "Portable Archive Exchange". This command is similar to "tar" and "cpio" commands for creating and managing archives. However, it has some functionality that these other commands do not have.

The pax command has several options that can be used with it. Below are some of the common ones:

-c: This option is used to create an archive. It takes a list of files/directories you want to archive and creates an archive file in your current directory. For example, "pax -c -f archive_file.tar file1.txt file2.txt"

-r: This option is used to append new files to an existing archive. For example, "pax -r -f archive_file.tar file3.txt"

-t: This option is used to list the contents of an archive. For example, "pax -t -f archive_file.tar"

-u: This option is used to update an archive. It replaces files in the archive with newer versions of those files. For example, "pax -u -f archive_file.tar file1.txt"

-x: This option is used to extract files from an archive. For example, "pax -x -f archive_file.tar".

In addition to the above options, pax offers several additional options for handling file permissions, directory structure, and symbolic links.

Overall, the pax command is a powerful tool for archiving files in various formats and can be used as an alternative to other archive commands like "tar" and "cpio". 

## tldr 
 
> Archiving and copying utility.
> More information: <https://manned.org/pax.1p>.

- List the contents of an archive:

`pax -f {{archive.tar}}`

- List the contents of a gzipped archive:

`pax -zf {{archive.tar.gz}}`

- Create an archive from files:

`pax -wf {{target.tar}} {{path/to/file1}} {{path/to/file2}} {{path/to/file3}}`

- Create an archive from files, using output redirection:

`pax -w {{path/to/file1}} {{path/to/file2}} {{path/to/file3}} > {{target.tar}}`

- Extract an archive into the current directory:

`pax -rf {{source.tar}}`

- Copy to a directory, while keeping the original metadata; `target/` must exist:

`pax -rw {{path/to/file1}} {{path/to/directory1}} {{path/to/directory2}} {{target/}}`
