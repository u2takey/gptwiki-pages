# md5sum 
## chatgpt 
The "md5sum" command is a Linux command used to calculate the MD5 checksum of a file. An MD5 checksum is a 128-bit cryptographic hash that is used to verify the integrity of a file. To use the "md5sum" command, simply type "md5sum" followed by the name of the file you wish to calculate the checksum for. The command will then generate a string of characters that represents the MD5 checksum for the file. This string can be compared to the MD5 checksum provided by the file's creator to ensure that the file has not been modified or corrupted. The "md5sum" command can be particularly useful when downloading large files or software packages, as it provides a way to verify that the downloaded file is the same as the original file. 

## tldr 
 
> Calculate MD5 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/md5sum>.

- Calculate the MD5 checksum for a file:

`md5sum {{path/to/file}}`

- Calculate MD5 checksums for multiple files:

`md5sum {{path/to/file1}} {{path/to/filen2}}`

- Calculate a MD5 checksum from the standard input:

`echo "{{text}}" | md5sum`

- Read a file of MD5SUMs and verify all files have matching checksums:

`md5sum --check {{path/to/file.md5}}`

- Only show a message for missing files or when verification fails:

`md5sum --check --quiet {{path/to/file.md5}}`

- Only show a message for files for which verification fails, ignoring missing files:

`md5sum --ignore-missing --check --quiet {{path/to/file.md5}}`
