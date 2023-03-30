# engrampa 
## chatgpt 
Engrampa is a command-line file archiver and compressor that is used to create, extract, and manage archive files on a Linux system. It is the default archive manager of the MATE desktop environment and is based on the highly renowned file archiver "File Roller". Engrampa has a simple user interface and supports a wide range of archive formats such as ZIP, TAR, GZIP, BZIP, etc.

When you run the command "engrampa" on a Linux terminal, it launches the Engrampa application, which provides you with various options to compress or decompress files and folders, create and extract archives, add, delete or view files within an archive, etc. Engrampa can be used to protect archive files with passwords or encryption, and also to split large files into smaller parts for easy transfer or storage.

Overall, Engrampa is a valuable tool that allows users to compress, decompress, and manage archived data using an intuitive and user-friendly interface on their Linux system. 

## tldr 
 
> Package files into zip/tar file in MATE desktop environment.
> See also: `zip`, `tar`.
> More information: <https://github.com/mate-desktop/engrampa>.

- Start engrampa:

`engrampa`

- Open specific archives:

`engrampa {{path/to/archive1.tar path/to/archive2.tar ...}}`

- Archive specific files and/or directories recursively:

`engrampa --add-to={{path/to/compressed.tar}} {{path/to/file_or_directory1 path/to/file_or_directory2 ...}}`

- Extract files and/or directories from archives to a specific path:

`engrampa --extract-to={{path/to/directory}} {{path/to/archive1.tar path/to/archive2.tar ...}}`
