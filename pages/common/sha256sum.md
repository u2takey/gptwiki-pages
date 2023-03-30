# sha256sum 
## chatgpt 
The `sha256sum` command is a utility program in Linux and other Unix-like operating systems that generates and verifies SHA-256 checksums, which are a type of digital signature used to verify the integrity of files. A checksum is a unique, fixed-size value computed from a file's contents using a mathematical algorithm, in this case SHA-256, which is a cryptographic hash function.

To generate a SHA-256 checksum for a file using the `sha256sum` command, you can type the following command in a terminal or command prompt:

`sha256sum filename`

Replace `filename` with the name of the file you wish to generate a checksum for. The command will calculate the SHA-256 checksum of the file and display it in the terminal window along with the file name. This checksum can be used to verify that the file has not been altered or corrupted.

To verify the integrity of a file using its SHA-256 checksum, you can use the following command:

`sha256sum -c filename.sha256`

Replace `filename` with the name of the file you wish to verify, and `filename.sha256` with the name of the file containing the checksum. The command will calculate the SHA-256 checksum of the file and compare it to the checksum in the `.sha256` file. If the two checksums match, the file has not been altered or corrupted. If they don't match, the file may have been tampered with or corrupted.

In summary, `sha256sum` is a command-line utility used to generate and verify SHA-256 checksums in Linux and other Unix-like operating systems. It is a useful tool for verifying the integrity of files downloaded from the Internet or transferred from one system to another. 

## tldr 
 
> Calculate SHA256 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/manual/html_node/sha2-utilities.html>.

- Calculate the SHA256 checksum for a file:

`sha256sum {{path/to/file}}`

- Calculate SHA256 checksums for multiple files:

`sha256sum {{path/to/file1}} {{path/to/file2}}`

- Calculate and save the list of SHA256 checksums to a file:

`sha256sum {{path/to/file1}} {{path/to/file2}} > {{path/to/file.sha256}}`

- Read a file of SHA256 sums and verify all files have matching checksums:

`sha256sum --check {{path/to/file.sha256}}`

- Only show a message for missing files or when verification fails:

`sha256sum --check --quiet {{path/to/file.sha256}}`

- Only show a message for files for which verification fails, ignoring missing files:

`sha256sum --ignore-missing --check --quiet {{path/to/file.sha256}}`
