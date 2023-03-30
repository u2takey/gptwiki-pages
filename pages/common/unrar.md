# unrar 
## chatgpt 
The "unrar" command is a terminal/command-line utility for extracting or unrar'ing files that have been archived in the RAR format. The RAR format is commonly used for compressing files and folders into a single file, making them easier to transfer or store. 

The "unrar" command is used to extract the contents of such a RAR archive into a folder or location on your computer. The basic syntax of the command is as follows:

unrar e [options] file.rar [destination]

Where "e" stands for "extract", "file.rar" is the name of the archive to be extracted, and "[destination]" is the folder/location where the extracted files will be saved. The command also offers various options that can be used to customize the extraction process, like selecting specific files to extract or creating new subfolders for the extracted files. 

Some examples of how to use the "unrar" command:

- To extract a RAR archive named "file.rar" to the current directory: 
unrar e file.rar 

- To extract the archive to a specific directory, say "/home/user/folder":
unrar e file.rar /home/user/folder

- To extract only a specific file from the archive, say "my_file.txt":
unrar e file.rar my_file.txt

Overall, the "unrar" command is a powerful utility for dealing with RAR archives in the terminal/command-line environment.  It can be a useful tool for managing and organizing large files. 

## tldr 
 
> Extract RAR archives.
> More information: <https://manned.org/unrar>.

- Extract files with original directory structure:

`unrar x {{compressed.rar}}`

- Extract files to a specified path with the original directory structure:

`unrar x {{compressed.rar}} {{path/to/extract}}`

- Extract files into current directory, losing directory structure in the archive:

`unrar e {{compressed.rar}}`

- Test integrity of each file inside the archive file:

`unrar t {{compressed.rar}}`

- List files inside the archive file without decompressing it:

`unrar l {{compressed.rar}}`
