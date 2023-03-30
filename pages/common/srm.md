# srm 
## chatgpt 
The command "srm" is used in Unix and Unix-based systems, including macOS. It stands for "Secure Removal" and is used to securely delete files or directories from a system, making sure that they cannot be recovered by any means. The command overwrites the file or directory with random data, which makes it unrecoverable.

Here are the parameters that can be used with the "srm" command:

- "-z" or "--zero": It overwrites the file with zeroes instead of random data.
- "-f" or "--force": It forces the removal of files without prompting the user for confirmation.
- "-r" or "-R" or "--recursive": It recursively deletes directories.
- "-l" or "--local": It deletes the local copy of a file that has been synchronized with a remote copy.
- "-v" or "--verbose": It displays the progress and information about the operation.
- "-s" or "--simple": It overwrites the file with a single pass instead of the default of seven passes.

Example usage:

To securely delete a file using the default settings, you can use the following command:

`srm example_file.txt`

To securely delete a directory and its contents, you can use the following command:

`srm -r example_directory/` 

To securely delete a file with a single pass, you can use the following command:

`srm -s example_file.txt` 

Overall, the "srm" command is a powerful tool for destroying sensitive data from a system with security in mind. However, always use it with caution as data once deleted with this command cannot be recovered. 

## tldr 
 
> Securely remove files or directories.
> Overwrites the existing data one or multiple times. Drop in replacement for rm.
> More information: <http://srm.sourceforge.net/srm.html>.

- Remove a file after a single-pass overwriting with random data:

`srm -s {{path/to/file}}`

- Remove a file after seven passes of overwriting with random data:

`srm -m {{path/to/file}}`

- Recursively remove a directory and its contents overwriting each file with a single-pass of random data:

`srm -r -s {{path/to/directory}}`

- Prompt before every removal:

`srm -i {{\*}}`
