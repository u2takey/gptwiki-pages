# sha512sum 
## chatgpt 
`sha512sum` is a Linux command used to calculate a SHA-512 message digest of a file. SHA-512 is a cryptographic hash function that generates a 512-bit hash value, which is a fixed-size output. A hash value is a unique digital fingerprint of the input file.

The command syntax is as follows:

```
sha512sum [OPTION]... [FILE]...
```

The `[OPTION]` parameter is optional and allows you to modify the behavior of the command. Here are some commonly used options:

- `-c` or `--check`: read SHA-512 checksums from the specified file(s) and check them against the calculated checksums
- `-b` or `--binary`: read in binary mode instead of text mode
- `-t` or `--text`: read in text mode (default)

The `[FILE]` parameter specifies the file(s) for which you want to calculate the SHA-512 checksums.

When you run the `sha512sum` command without any options or arguments, it reads from standard input and calculates the SHA-512 message digest of the input data.

The output of the `sha512sum` command is a string that contains the calculated SHA-512 checksum followed by the file name. For example:

```
f5a5b5a8a3c15d38cf679d5ae789991f2768e1e9b67a702fb3322fc7d25dbf8b5032c1d9012787b15e923cb3335887c9fa01d6aca7afdf5a3a8f3de0f0f480b1  example.txt
```

The first part of the string is the SHA-512 checksum, and the second part is the file name.

The `sha512sum` command is often used to verify the integrity of downloaded files or to ensure that files have not been modified since they were created. To do this, you would calculate the SHA-512 checksum of the original file and compare it to the checksum of the downloaded or modified file. If the two checksums match, it indicates that the files are identical. 

## tldr 
 
> Calculate SHA512 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

- Calculate the SHA512 checksum for a file:

`sha512sum {{path/to/file}}`

- Calculate SHA512 checksums for multiple files:

`sha512sum {{path/to/file1}} {{path/to/file2}}`

- Calculate and save the list of SHA512 checksums to a file:

`sha512sum {{path/to/file1}} {{path/to/file2}} > {{path/to/file.sha512}}`

- Read a file of SHA512 sums and verify all files have matching checksums:

`sha512sum --check {{path/to/file.sha512}}`

- Only show a message for missing files or when verification fails:

`sha512sum --check --quiet {{path/to/file.sha512}}`

- Only show a message for files for which verification fails, ignoring missing files:

`sha512sum --ignore-missing --check --quiet {{path/to/file.sha512}}`
