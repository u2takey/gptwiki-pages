# sha224sum 
## chatgpt 
The command `sha224sum` is a Linux command that is used to calculate and display the SHA-224 checksum of a file. The SHA-224 algorithm is a secure hash algorithm that takes an input file and generates a unique fixed-size output, known as a checksum or digest. The checksum can be used to verify the integrity of the file, as any changes made to the file after the checksum was calculated will result in a different checksum.

The syntax of the `sha224sum` command is as follows:

```
sha224sum [OPTION]... [FILE]...
```

The `OPTION` parameter is optional and can be used to modify the behavior of the command. The `FILE` parameter is required and specifies the file or files for which the checksum should be calculated.

The `sha224sum` command generates a message digest for each specified file and outputs the digest along with the filename to the standard output.

Example:

```
$ sha224sum myfile.txt
4ea91b252ce6e696d67abbd2a95bbe3f35e9fe8ed26e018c7826da7f

```

In the above example, the `sha224sum` command is used to calculate the SHA-224 checksum of the `myfile.txt` file, and the resulting checksum is displayed on the screen.

Some of the commonly used options for the `sha224sum` command are as follows:

- `-c`: Reads the checksums from a file and verifies them against the specified files.
- `-b`: Outputs the checksums in binary format instead of hexadecimal format.
- `-t`: Outputs the checksums in a format that is compatible with the traditional Unix `sum` command.

Overall, the `sha224sum` command is a useful tool for verifying the integrity of files and ensuring that they have not been tampered with. 

## tldr 
 
> Calculate SHA224 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

- Calculate the SHA224 checksum for a file:

`sha224sum {{path/to/file}}`

- Calculate SHA224 checksums for multiple files:

`sha224sum {{path/to/file1}} {{path/to/file2}}`

- Calculate and save the list of SHA224 checksums to a file:

`sha224sum {{path/to/file1}} {{path/to/file2}} > {{path/to/file.sha224}}`

- Read a file of SHA224 sums and verify all files have matching checksums:

`sha224sum --check {{path/to/file.sha224}}`

- Only show a message for missing files or when verification fails:

`sha224sum --check --quiet {{path/to/file.sha224}}`

- Only show a message for files for which verification fails, ignoring missing files:

`sha224sum --ignore-missing --check --quiet {{path/to/file.sha224}}`
