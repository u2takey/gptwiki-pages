# sha1sum 
## chatgpt 
The `sha1sum` command is a Linux command that is used to calculate and display the SHA-1 hash value of a file or input. The SHA-1 algorithm is a hashing algorithm that generates a unique 160-bit hash value for a given file or input. 

To use the `sha1sum` command, you need to specify the file or input whose hash value you want to calculate. For example, if you want to calculate the hash value of a file called "myfile.txt", you would run the command:

```
sha1sum myfile.txt
```

The output of the command will be a string of 40 hexadecimal digits that represents the SHA-1 hash value of the file. This hash value can be used to verify the authenticity of the file or to check if it has been tampered with.

Additionally, the `sha1sum` command can be used to verify the integrity of a file. This is done by comparing the calculated hash value with the known hash value of the file. If the two values match, it means that the file has not been changed or corrupted.

In summary, the `sha1sum` command is a useful tool for verifying the integrity of files and ensuring their authenticity. 

## tldr 
 
> Calculate SHA1 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/sha1sum>.

- Calculate the SHA1 checksum for a file:

`sha1sum {{path/to/file}}`

- Calculate SHA1 checksums for multiple files:

`sha1sum {{path/to/file1}} {{path/to/file2}}`

- Calculate and save the list of SHA1 checksums to a file:

`sha1sum {{path/to/file1}} {{path/to/file2}} > {{path/to/file.sha1}}`

- Read a file of SHA1 sums and verify all files have matching checksums:

`sha1sum --check {{path/to/file.sha1}}`

- Only show a message for missing files or when verification fails:

`sha1sum --check --quiet {{path/to/file.sha1}}`

- Only show a message for files for which verification fails, ignoring missing files:

`sha1sum --ignore-missing --check --quiet {{path/to/file.sha1}}`
