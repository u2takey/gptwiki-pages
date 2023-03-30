# zip2john 
## chatgpt 
zip2john is a command-line utility that is used to extract the hash of a password-protected ZIP file. It works by converting the password-protected archive into a format that can be read and cracked by password cracking tools like John the Ripper.

The complete syntax of the zip2john command is as follows:

```
zip2john [options] zipfile > outputfile
```

Here, the `[options]` refer to any optional arguments that can be passed to the command. The `zipfile` argument specifies the path to the ZIP file that needs to be cracked. The `outputfile` argument specifies the name of the file where the hash output will be saved.

To use the zip2john command, you first need to navigate to the directory that contains the ZIP file that needs to be cracked. Once you're in the correct directory, you can run the zip2john command with the appropriate arguments.

After running the zip2john command, it will extract the hash of the password-protected ZIP file and save it to the output file specified in the command. This output file can then be used as an input for password cracking tools like John the Ripper, to try and crack the password.

In summary, zip2john is a command-line utility that extracts the hash of a password-protected ZIP file and saves it to a file, which can be used for password cracking. 

## tldr 
 
> A tool to extract password hashes from zip files for use with John the Ripper password cracker.
> This is a utility tool usually installed as part of the John the Ripper installation.
> More information: <https://www.openwall.com/john/>.

- Extract the password hash from an archive, listing all files in the archive:

`zip2john {{path/to/file.zip}}`

- Extract the password hash using [o]nly a specific compressed file:

`zip2john -o {{path/to/compressed_file}} {{path/to/file.zip}}`

- Extract the password hash from a compressed file to a specific file (for use with John the Ripper):

`zip2john -o {{path/to/compressed_file}} {{path/to/file.zip}} > {{file.hash}}`
