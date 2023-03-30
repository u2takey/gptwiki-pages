# shred 
## chatgpt 
Shred is a command-line utility that securely deletes files in a manner that prevents them from being recovered by any means. The command works by overwriting the data in a file with random data multiple times, making it virtually impossible for anyone to recover the original file. 

Here is the syntax of the shred command:

shred [OPTIONS] [FILE(s)]

Some common options used with the “shred” command are:

-f, --force: Forces the overwrite of read-only files and folders.
-u, --remove: Truncate and remove the file after overwriting.
-v, --verbose: Show progress details of overwriting procedures.
-n, --iterations=N: Specifies N, the number of times the data in the file should be overwritten. By default, this option is set to 3.
-z: After overwriting the files, write zeros instead.

To use the shred command, simply specify the file name with the command. For example, to securely delete a file named "mypersonaldocuments.docx," the command line would be:

shred mypersonaldocuments.docx

This will overwrite the file three times by default and leave no traceable data that can be recovered from the file. 

It is noteworthy that some file systems do not support data deletion by default at the hardware level, in this case, using shred will not guarantee that the data is removed from the hardware level. 

## tldr 
 
> Overwrite files to securely delete data.
> More information: <https://www.gnu.org/software/coreutils/shred>.

- Overwrite a file:

`shred {{path/to/file}}`

- Overwrite a file, leaving zeroes instead of random data:

`shred --zero {{path/to/file}}`

- Overwrite a file 25 times:

`shred -n25 {{path/to/file}}`

- Overwrite a file and remove it:

`shred --remove {{path/to/file}}`
