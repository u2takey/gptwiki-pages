# shasum 
## chatgpt 
The `shasum` command is a Unix utility that is used to compute and verify SHA checksums of files on a Unix-like operating system. The command takes a filename or a list of filenames and calculates the SHA checksum of each file. The computed SHA checksum is displayed as a 40-character hexadecimal string. SHA-1 is the default algorithm used by `shasum`, but various other SHA algorithms, such as SHA-256, SHA-384, and SHA-512 can also be used with the relevant options.

Sha checksums are used to verify the integrity of a file. A checksum is a small fixed-size datum derived from a block of digital data for the purpose of detecting errors that may have been introduced during its transmission or storage. By checking the checksum of a file, you can ensure that the file has not been modified or corrupted in any way.

Here's an example of how to use the `shasum` command:

```sh
shasum -a 256 myfile.txt
```

In this case, we're calculating the SHA-256 checksum of a file called `myfile.txt`.

The `-a` option specifies the algorithm to use, which in this case is SHA-256. `shasum` will then output the checksum for that file.

It's important to note that checksums only verify the integrity of a file, and not its authenticity. If you want to verify the authenticity of a file, you need to use a digital signature or some other form of authentication. 

## tldr 
 
> Calculate or check cryptographic SHA checksums.
> More information: <https://manned.org/shasum>.

- Calculate the SHA1 checksum for a file:

`shasum {{path/to/file}}`

- Calculate the SHA256 checksum for a file:

`shasum --algorithm 256 {{path/to/file}}`

- Calculate the SHA512 checksum for multiple files:

`shasum --algorithm 512 {{path/to/file1}} {{path/to/file2}}`

- Calculate and save the list of SHA256 checksums to a file:

`shasum --algorithm 256 {{path/to/file1}} {{path/to/file2}} > {{path/to/file.sha256}}`

- Check a file with a list of sums against the directory's files:

`shasum --check {{path/to/file}}`

- Check a list of sums and only show a message for files for which verification fails:

`shasum --check --quiet {{path/to/file}}`

- Calculate the SHA1 checksum from `stdin`:

`{{some_command}} | shasum`
