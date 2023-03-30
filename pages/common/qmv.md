# qmv 
## chatgpt 
The qmv command is used to edit and rename multiple files in an email-based interface. It is a part of the renameutils package and is used to process files interactively through your email client.

Here is how to use the qmv command:

1. Install the renameutils package on your system.

2. Open a terminal window and navigate to the directory where the files you want to rename are stored.

3. Type the command qmv followed by a space and a wildcard (*) to select all the files you want to rename.

4. Press enter, and the files will open in your default email client in a table format.

5. Edit the names of the files in the table by modifying the text in the "new name" column.

6. Save the changes to the table and close your email client.

7. The qmv command will apply the new names to the files you renamed.

In summary, the qmv command allows you to rename multiple files interactively through your email client by presenting them in a table format for easy editing. With this command, you can rename files quickly and efficiently. 

## tldr 
 
> Move files and directories using the default text editor to define the filenames.
> More information: <https://www.nongnu.org/renameutils/>.

- Move a single file (open an editor with the source filename on the left and the target filename on the right):

`qmv {{source_file}}`

- Move multiple JPG files:

`qmv {{*.jpg}}`

- Move multiple directories:

`qmv -d {{path/to/directory1}} {{path/to/directory2}} {{path/to/directory3}}`

- Move all files and directories inside a directory:

`qmv --recursive {{path/to/directory}}`

- Move files, but swap the positions of the source and the target filenames in the editor:

`qmv --option swap {{*.jpg}}`

- Rename all files and folders in the current directory, but show only target filenames in the editor (you can think of it as a kind of simple mode):

`qmv --format=do .`
