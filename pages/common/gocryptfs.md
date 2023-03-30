# gocryptfs 
## chatgpt 
gocryptfs is a command line tool for creating and mounting encrypted filesystems in Linux. Here is a brief explanation of the command:

Syntax:
```
gocryptfs [options] mountpoint
```
The command requires the following parameters:

- `[options]`: optional parameters for customizing the encryption process.
- `mountpoint`: the directory where the encrypted filesystem will be mounted.

Options:

- `-init`: creates a new encrypted filesystem.
- `-config=path`: set a custom config file path.
- `-nofail`: do not fail if the mountpoint already exists.
- `-reverse`: mount the filesystem in reverse mode, which allows the unencrypted data to be modified on-the-fly.

Examples:

1. Initialize a new encrypted filesystem:
```
gocryptfs -init ~/private
```
This will create a new encrypted filesystem in the `~/private` directory.

2. Mount an existing encrypted filesystem:
```
gocryptfs ~/private ~/private-mount
```
This will mount the encrypted filesystem located in `~/private` to the `~/private-mount` directory.

3. Mount an encrypted filesystem in reverse mode:
```
gocryptfs -reverse ~/private ~/reverse-mount
```
This will mount the encrypted filesystem located in `~/private` to the `~/reverse-mount` directory in reverse mode. 

## tldr 
 
> Encrypted overlay filesystem written in Go.
> More information: <https://github.com/rfjakob/gocryptfs>.

- Initialize an encrypted filesystem:

`gocryptfs -init {{path/to/cipher_dir}}`

- Mount an encrypted filesystem:

`gocryptfs {{path/to/cipher_dir}} {{path/to/mount_point}}`

- Mount with the explicit master key instead of password:

`gocryptfs --masterkey {{path/to/cipher_dir}} {{path/to/mount_point}}`

- Change the password:

`gocryptfs --passwd {{path/to/cipher_dir}}`

- Make an encrypted snapshot of a plain directory:

`gocryptfs --reverse {{path/to/plain_dir}} {{path/to/cipher_dir}}`
