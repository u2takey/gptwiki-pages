# b2sum 
## chatgpt 
b2sum is a command-line utility in Linux and other Unix-like operating systems that computes and displays a hash value of the input file in BLAKE2 format. This command is used to verify the integrity of files and/or to detect any changes to its contents. 

The syntax of the b2sum command is as follows:
```
b2sum [OPTIONS] [FILES]
```

Here, OPTIONS include various flags that can be used with the command, and FILES indicate the files whose hash values are to be computed. 

Some commonly used options with b2sum are:

- -c or --check: Instructs the command to read the hash sums from a file and verify whether the input files have the same hash values.
- -l or --length: Displays the length of the BLAKE2 hash function in bytes.
- -s or --simple: Produces a simpler, more concise output format.

For example, to compute the BLAKE2 hash value of a file named myfile.txt, the following command can be used:
```
b2sum myfile.txt
```

This will display the hash value of the file along with its filename.

To check the integrity of a file, we can first create a checksum file using the following command:
```
b2sum myfile.txt > myfile_checksum.txt
```

This will create a file myfile_checksum.txt containing the hash value of myfile.txt. To verify whether myfile.txt is intact, we can use the following command:
```
b2sum -c myfile_checksum.txt
```

This will compare the hash value of myfile.txt with its expected checksum value in myfile_checksum.txt and indicate whether they match or not. If the checksum matches, the file is not corrupted, and its contents are intact. 

## tldr 
 
> Calculate BLAKE2 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/b2sum>.

- Calculate the BLAKE2 checksum for a file:

`b2sum {{path/to/file}}`

- Calculate BLAKE2 checksums for multiple files:

`b2sum {{path/to/file1}} {{path/to/file2}}`

- Calculate the BLAKE2 checksum from `stdin`:

`{{some_command}} | b2sum`

- Read a file of BLAKE2 sums and filenames and verify all files have matching checksums:

`b2sum --check {{path/to/file.b2}}`

- Only show a message for missing files or when verification fails:

`b2sum --check --quiet {{path/to/file.b2}}`

- Only show a message for files for which verification fails, ignoring missing files:

`b2sum --ignore-missing --check --quiet {{path/to/file.b2}}`
