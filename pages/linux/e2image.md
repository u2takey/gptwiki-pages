# e2image 
## chatgpt 
The e2image command is used in Linux operating systems to create an image of a valid ext2, ext3, or ext4 file system. It creates an image of the file system in a file format that can later be used to restore the original file system state.

The basic syntax of the e2image command is:

e2image [options] device filename

Where device is the block device that contains the file system to be imaged and filename is the name of the file in which the image will be stored.

Some of the common options used with the e2image command include:

- -r : This option allows the imaging of a file system that is mounted read-only.
- -p : This option creates a compressed image of the file system.
- -c : This option creates a clone of the file system, including all subdirectories and files.
- -t : This option creates a text file containing metadata about the file system.
- -S : This option skips the imaging of free space on the file system.

The e2image command is a powerful tool that allows system administrators to back up file systems and restore them in case of system failure. It can also be used to create a portable copy of a file system that can be easily transferred to another computer. 

## tldr 
 
> Save critical ext2/ext3/ext4 filesystem metadata to a file.
> More information: <https://manned.org/e2image>.

- Write metadata located on device to a specific file:

`e2image {{/dev/sdXN}} {{path/to/image_file}}`

- Print metadata located on device to `stdout`:

`e2image {{/dev/sdXN}} -`

- Restore the filesystem metadata back to the device:

`e2image -I {{/dev/sdXN}} {{path/to/image_file}}`

- Create a large raw sparse file with metadata at proper offsets:

`e2image -r {{/dev/sdXN}} {{path/to/image_file}}`

- Create a QCOW2 image file instead of a normal or raw image file:

`e2image -Q {{/dev/sdXN}} {{path/to/image_file}}`
