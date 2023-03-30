# mmv 
## chatgpt 
The mmv command is a Linux utility that is used to move, rename, or manipulate multiple files at once. It is a powerful tool that saves time and effort as it allows the user to apply the same action on multiple files in one go.

Syntax:
mmv [-v] [-n] source target

Options:
-v: Activate verbose mode which displays detailed output.
-n: Enable no-act mode which lists the operations that would have taken place but does not execute them.

Usage:
To rename a single file, the syntax is as follows:
mmv oldname newname

To rename or move multiple files, we use wildcard characters to select the files we want to modify. For example:
mmv *.txt /dir/newname*.txt
This command renames all files with text extension in the current directory to a new name and moves them to the /dir/ directory.

Overall, the mmv command is an efficient and convenient tool for batch renaming files quickly on the command line. 

## tldr 
 
> Move and rename files in bulk.
> More information: <https://manned.org/mmv.1>.

- Rename all files with a certain extension to a different extension:

`mmv "*{{.old_extension}}" "#1{{.new_extension}}"`

- Copy `report6part4.txt` to `./french/rapport6partie4.txt` along with all similarly named files:

`mmv -c "{{report*part*.txt}}" "{{./french/rapport#1partie#2.txt}}"`

- Append all `.txt` files into one file:

`mmv -a "{{*.txt}}" "{{all.txt}}"`

- Convert dates in filenames from "M-D-Y" format to "D-M-Y" format:

`mmv "{{[0-1][0-9]-[0-3][0-9]-[0-9][0-9][0-9][0-9].txt}}" "{{#3#4-#1#2-#5#6#7#8.txt}}"`
