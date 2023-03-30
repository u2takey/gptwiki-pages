# touch 
## chatgpt 
The touch command is used in Unix-based operating systems to create an empty file or update the access and modification timestamps of a file. 

The syntax for the touch command is:

touch [OPTION]... [FILE]...

The possible options that can be used with the touch command are:

- -a: Change only the access time of the file.
- -c: Do not create the file if it does not already exist.
- -d <DATE_STRING>: Use the specified date and time instead of the current time. The DATE_STRING must be in the format "+%Y-%m-%d %H:%M:%S".
- -m: Change only the modification time of the file.
- -r <REFERENCE_FILE>: Use the access and modification times of the reference file instead of the current time.
- --help: Display the help message and exit.
- --version: Display the version information and exit.

The touch command is most commonly used to create an empty file. If you specify the name of a file that does not exist, touch will create an empty file with that name. For example:

touch myfile.txt

If you want to update the access and modification timestamps of an existing file, you can use the -a and -m options, respectively. For example:

touch -a myfile.txt
touch -m myfile.txt

You can also use the -r option to set the access and modification times of a file to be the same as another file. For example:

touch -r reference.txt myfile.txt

Overall, the touch command is a simple yet powerful tool for manipulating file timestamps in Unix-based operating systems. 

## tldr 
 
> Create files and set access/modification times.
> More information: <https://manned.org/man/freebsd-13.1/touch>.

- Create specific files:

`touch {{path/to/file1 path/to/file2 ...}}`

- Set the file [a]ccess or [m]odification times to the current one and don't [c]reate file if it doesn't exist:

`touch -c -{{a|m}} {{path/to/file1 path/to/file2 ...}}`

- Set the file [t]ime to a specific value and don't [c]reate file if it doesn't exist:

`touch -c -t {{YYYYMMDDHHMM.SS}} {{path/to/file1 path/to/file2 ...}}`

- Set the file time of a specific file to the time of anothe[r] file and don't [c]reate file if it doesn't exist:

`touch -c -r {{~/.emacs}} {{path/to/file1 path/to/file2 ...}}`
