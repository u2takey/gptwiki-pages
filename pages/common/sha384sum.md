# sha384sum 
## chatgpt 
The "sha384sum" command is used to calculate the SHA-384 message digest of a file. 

SHA-384 is a cryptographic hash function that takes an input (in this case, a file) and produces a fixed-size output (384 bits) that is unique for that input. This output, also known as the hash value or message digest, can be used to verify the integrity of the original file, as any modification to the file will result in a different hash value.

The syntax for the "sha384sum" command is:

sha384sum [OPTION]... [FILE]...

Where [OPTION] refers to any optional parameters that can be used with the command, and [FILE] refers to the file(s) for which the SHA-384 hash is to be calculated.

Some common options for "sha384sum" include:

- -b, --binary: interpret the input files in binary mode
- -c, --check: read the SHA-384 sums from a file and check them against the calculated sums
- -t, --text: interpret the input files as text files
- -v, --verbose: print the name of each file before calculating its hash value

For example, to calculate the SHA-384 hash value of a file named "example.txt" and display the result in binary format, we can use the following command:

sha384sum -b example.txt

The output will be a line consisting of the hash value and the file name, separated by a space:

22a6b729dd786326b7c429d0f2bd7f9ac52dc8311c815f41493199f51c6d3570696b9131567d82bea2c1947abbd6cde1 example.txt 

## tldr 
 
> Calculate SHA384 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

- Calculate the SHA384 checksum for a file:

`sha384sum {{path/to/file}}`

- Calculate SHA384 checksums for multiple files:

`sha384sum {{path/to/file1}} {{path/to/file2}}`

- Calculate and save the list of SHA384 checksums to a file:

`sha384sum {{path/to/file1}} {{path/to/file2}} > {{path/to/file.sha384}}`

- Read a file of SHA384 sums and verify all files have matching checksums:

`sha384sum --check {{path/to/file.sha384}}`

- Only show a message for missing files or when verification fails:

`sha384sum --check --quiet {{path/to/file.sha384}}`

- Only show a message for files for which verification fails, ignoring missing files:

`sha384sum --ignore-missing --check --quiet {{path/to/file.sha384}}`
