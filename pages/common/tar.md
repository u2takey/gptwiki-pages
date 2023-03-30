# tar 
## chatgpt 
tar stands for Tape Archive, which is a command-line utility tool used for archiving files and directories in a computer. It is commonly used in Unix and Unix-like operating systems because it is capable of creating a single file that contains multiple files and directories while preserving their original file permissions, ownerships, and timestamps.

The basic syntax of the tar command is as follows:

tar [options] [archive_name] [files/directories to be archived]

Some of the commonly used options are:

-c: This option is used to create a new archive.

-x: This option is used to extract an archive.

-t: This option is used to view the contents of an archive.

-v: This option is used for verbose output, meaning it displays detailed information about the files being archived or extracted.

-f: This option is used to specify the name and location of the archive file.

-z: This option is used to compress the archive file using gzip.

-j: This option is used to compress the archive file using bzip2.

Some examples of the tar command in action are:

To create a new archive file:

tar -cvf archive.tar file1.txt file2.txt dir1/

This command will create a new archive file named archive.tar and include the file1.txt, file2.txt, and the directory named dir1.

To extract contents from an archive file:

tar -xvf archive.tar

This command will extract all the contents from the archive file named archive.tar.

To compress the archive using gzip:

tar -cvzf archive.tar.gz file1.txt file2.txt dir1/

This command will create a new archive file named archive.tar.gz and include the file1.txt, file2.txt, and the directory named dir1. The option -z is used to compress the archive using gzip.

In summary, the tar command is a useful utility tool for archiving and compressing files and directories in a computer. 

## tldr 
 
> Archiving utility.
> Often combined with a compression method, such as gzip or bzip2.
> More information: <https://www.gnu.org/software/tar>.

- [c]reate an archive and write it to a [f]ile:

`tar cf {{path/to/target.tar}} {{path/to/file1 path/to/file2 ...}}`

- [c]reate a g[z]ipped archive and write it to a [f]ile:

`tar czf {{path/to/target.tar.gz}} {{path/to/file1 path/to/file2 ...}}`

- [c]reate a g[z]ipped archive from a directory using relative paths:

`tar czf {{path/to/target.tar.gz}} --directory={{path/to/directory}} .`

- E[x]tract a (compressed) archive [f]ile into the current directory [v]erbosely:

`tar xvf {{path/to/source.tar[.gz|.bz2|.xz]}}`

- E[x]tract a (compressed) archive [f]ile into the target directory:

`tar xf {{path/to/source.tar[.gz|.bz2|.xz]}} --directory={{path/to/directory}}`

- [c]reate a compressed archive and write it to a [f]ile, using [a]rchive suffix to determine the compression program:

`tar caf {{path/to/target.tar.xz}} {{path/to/file1 path/to/file2 ...}}`

- Lis[t] the contents of a tar [f]ile [v]erbosely:

`tar tvf {{path/to/source.tar}}`

- E[x]tract files matching a pattern from an archive [f]ile:

`tar xf {{path/to/source.tar}} --wildcards "{{*.html}}"`
