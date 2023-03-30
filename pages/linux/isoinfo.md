# isoinfo 
## chatgpt 
Isoinfo is a command line tool used to extract information from ISO 9660 CD-ROM image files, which are a common format for distributing software and operating system installation files.

The isoinfo command has a few different options that can be used to extract various types of information from the ISO file. Here are some of the most commonly used options along with their descriptions:

-l: Lists the contents of the ISO file, including file names, sizes, and permissions.

-j: Lists the Joliet extension data associated with the ISO file, which provides support for long file names and various international characters.

-i: Specifies the location of the ISO file to extract information from.

-d: Enables debug output, which can be useful for troubleshooting issues with the ISO file.

-f: Specifies a file within the ISO file to extract information about.

-h: Displays help information about the isoinfo command and its various options.

Overall, the isoinfo command is a useful tool for examining the contents of ISO files, which can be especially helpful when troubleshooting installation or configuration issues. 

## tldr 
 
> Utility programs for dumping and verifying ISO disk images.
> More information: <https://manned.org/isoinfo>.

- List all the files included in an ISO image:

`isoinfo -f -i {{path/to/image.iso}}`

- E[x]tract a specific file from an ISO image and send it out `stdout`:

`isoinfo -i {{path/to/image.iso}} -x {{/PATH/TO/FILE/INSIDE/ISO.EXT}}`

- Show header information for an ISO disk image:

`isoinfo -d -i {{path/to/image.iso}}`
