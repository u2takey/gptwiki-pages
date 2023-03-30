# mkisofs 
## chatgpt 
The mkisofs command is used to create an ISO 9660 file system image of a directory tree. ISO 9660 is a standard file system format used for CD-ROMs and other storage media.

The syntax of the mkisofs command is as follows:

mkisofs [options] -o output_file.iso source_directory

Here, the options are various parameters that define how the ISO file should be created, such as control over file names, file permissions, and directory structure. The source_directory parameter is the directory whose contents should be included in the ISO image.

When the command is executed, it will generate a single file named output_file.iso in the current directory. The resulting ISO image can be used to create a bootable CD or DVD, or as a data archive that can be burned to a disc or distributed electronically.

Some common options for the mkisofs command include:

- -r: Include permissions and ownership information for files
- -J: Use the Joliet file name extension for 8.3 filenames
- -l: Allow file names longer than 31 characters
- -o: Specify the output file name and location

Overall, the mkisofs command is a powerful tool for creating ISO images of directory trees, with many options available to customize the process. 

## tldr 
 
> Create ISO files from directories.
> Also aliased as `genisoimage`.
> More information: <https://manned.org/mkisofs>.

- Create an ISO from a directory:

`mkisofs -o {{filename.iso}} {{path/to/source_directory}}`

- Set the disc label when creating an ISO:

`mkisofs -o {{filename.iso}} -V "{{label_name}}" {{path/to/source_directory}}`
