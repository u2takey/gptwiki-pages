# atool 
## chatgpt 
The 'atool' command is a tool for managing file archives on Linux systems. It is a command-line utility that can handle various archive formats such as tar, zip, gzip, bzip2, cpio, rar, lha, and 7zip.

Here are some of the common tasks that can be performed using 'atool':

1. Archiving files: The atool command can be used to create archives of one or more files. For example, to create a tar archive of a directory named 'mydir', you can type the following command: atool -a mydir.tar mydir

2. Extracting files: At the same time, atool can be used to extract files from an existing archive. For example, to extract all files from a tar archive named 'myarchive.tar', you can type the following command: atool -x myarchive.tar

3. Testing archives: At times, you may need to verify the integrity of an archive. The atool command can be used for this purpose as well. To check the contents of a tar archive named 'myarchive.tar', you can type the following command: atool -t myarchive.tar

In addition to the above tasks, atool can also be used for viewing the contents of an archive, comparing two archives, and compression/decompression of files in the supported formats.

Overall, the 'atool' command is a useful tool for managing archive files on Linux systems, particularly for those who prefer using the command-line interface. 

## tldr 
 
> Manage archives of various formats.
> More information: <https://www.nongnu.org/atool/>.

- List files in a zip archive:

`atool --list {{path/to/archive.zip}}`

- Unpack a tar.gz archive into a new subdirectory (or current directory if it contains only one file):

`atool --extract {{path/to/archive.tar.gz}}`

- Create a new 7zip archive with two files:

`atool --add {{path/to/archive.7z}} {{path/to/file1 path/to/file2 ...}}`

- Extract all zip and rar archives in the current directory:

`atool --each --extract {{*.zip *.rar}}`
