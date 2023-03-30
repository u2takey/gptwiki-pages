# cryfs 
## chatgpt 
Cryfs is a command-line tool that provides encryption for files and folders. The main purpose of this tool is to ensure the confidentiality of sensitive data by encrypting it. Cryfs stands for cryptographic filesystem.

The basic syntax for the Cryfs command is:

`cryfs <source_dir> <mount_dir> [options]`

Here, `<source_dir>` is the directory that requires encryption, `<mount_dir>` is the directory where the encrypted files will be mounted, and `[options]` are the specific arguments or options that can be provided to customize the encryption.

Some of the commonly used options with Cryfs include:

- `-c` to create a new encrypted volume
- `-p` to change the password
- `-u` to unmount the encrypted volume
- `-q` to enable quiet mode

When a user runs the `cryfs` command with proper parameters and options, the tool will encrypt the files in the `source_dir` and mount the encrypted files in the `mount_dir` directory. The user can then access the encrypted files by navigating to the `mount_dir` directory.

Cryfs uses the cryptographic algorithms AES-256 (Advanced Encryption Standard) and SHA512 (Secure Hash Algorithm) to provide strong encryption. The tool also offers additional security features like plausibly deniable encryption and random padding. 

## tldr 
 
> A cryptographic filesystem for the cloud.
> More information: <https://www.cryfs.org/>.

- Mount an encrypted filesystem. The initialization wizard will be started on the first execution:

`cryfs {{path/to/cipher_dir}} {{path/to/mount_point}}`

- Unmount an encrypted filesystem:

`cryfs-unmount {{path/to/mount_point}}`

- Automatically unmount after ten minutes of inactivity:

`cryfs --unmount-idle {{10}} {{path/to/cipher_dir}} {{path/to/mount_point}}`

- Show a list of supported ciphers:

`cryfs --show-ciphers`
