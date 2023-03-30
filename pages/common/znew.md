# znew 
## chatgpt 
As an AI language model, I'm not sure what specific command you are asking about. However, "znew" is a basic command in the Linux operating system that is used to compress (or uncompress) files with the .Z extenstion using the Lempel-Ziv-Welch (LZW) algorithm. The command replaces the original compressed file with a new compressed file, which has a file name extension of .gz. 

The basic syntax of the command is:

znew [option] [filename]

Here, "option" specifies a set of parameters to customize the behavior of the command. For example, -f forces the compression process, overwriting any existing output file. Other options include -r to recursively compress all files in a directory, -n to specify the number of backup copies to be made, and -q to suppress the output messages.

"filename" is the name of the file to be compressed. Note that the file must have a .Z extension, or else the command will not recognize it as a valid input file.

Overall, the "znew" command is a simple and effective tool for compressing files in the Linux operating system, making them more efficient to store, transmit, and manipulate. 

## tldr 
 
> Recompress files from `.Z` to `.gz` format.
> More information: <https://manned.org/znew>.

- Recompress a file from `.Z` to `.gz` format:

`znew {{path/to/file1.Z}}`

- Recompress multiple files and display the achieved size reduction % per file:

`znew -v {{path/to/file1.Z}} {{path/to/file2.Z}} {{path/to/file3.Z}}`

- Recompress a file using the slowest compression method (for optimal compression):

`znew -9 {{path/to/file1.Z}}`

- Recompress a file, [K]eeping the `.Z` file if it is smaller than the `.gz` file:

`znew -K {{path/to/file1.Z}}`
