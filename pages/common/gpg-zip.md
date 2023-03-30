# gpg-zip 
## chatgpt 
The gpg-zip command is used to create an encrypted archive of one or multiple files and/or directories using GNU Privacy Guard (GPG) encryption. It is a wrapper script around the tar command, which is used to create a tape archive of files, and the GPG command, which is used for encryption and decryption.

The syntax of the gpg-zip command is as follows:

```
gpg-zip [options] archive.tar.gz
```

The options that can be used with gpg-zip command are:

- `-c, --create`: Create a new archive.
- `-j, --bzip2`: Use bzip2 compression with tar.
- `--compression`: Specify the compression algorithm to use.
- `-o, --output`: Write output to a file.
- `--gpg`: Specify the GPG options to use.
- `--encrypt`: Encrypt the archive using GPG.
- `--sign`: Sign the archive using GPG.
- `--armor`: Create an ASCII armored output.
- `--batch`: Use batch mode (useful for scripts).
- `--quiet`: Suppress normal output messages.
- `--verbose`: Print more detailed output messages.
- `--dry-run`: Show what would be done, but don't actually do it.
- `--help`: Show help message.

Here is an example of how to use the gpg-zip command to create an encrypted archive of a file:

``` 
gpg-zip --encrypt --output my_archive.tar.gz.gpg my_file.txt
```

This command will create a file called `my_archive.tar.gz.gpg` that contains `my_file.txt` encrypted with GPG. The user will be prompted to enter a passphrase to encrypt the file.

Overall, gpg-zip is a convenient way to create an encrypted archive of files and directories without having to manually encrypt each file individually. The resulting archive can be easily decrypted using GPG. 

## tldr 
 
> Encrypt files and directories in an archive using GPG.
> More information: <https://www.gnupg.org/documentation/manuals/gnupg/gpg_002dzip.html>.

- Encrypt a directory into `archive.gpg` using a passphrase:

`gpg-zip --symmetric --output {{archive.gpg}} {{path/to/directory}}`

- Decrypt `archive.gpg` into a directory of the same name:

`gpg-zip --decrypt {{path/to/archive.gpg}}`

- List the contents of the encrypted `archive.gpg`:

`gpg-zip --list-archive {{path/to/archive.gpg}}`
