# cryptsetup 
## chatgpt 
cryptsetup is a command-line tool used for managing encryption of block devices like hard drives, USB drives, and memory cards. It allows you to create, open, close, and manage encrypted volumes. 

The syntax of the command is as follows:

```
cryptsetup <options> <action> <device> [keyfile]
```

where,
- options: Optional parameters to customize the behavior of the command.
- action: The operation to perform on the specified device, like create, open, close, or resize.
- device: The path to the block device for which the encryption will be managed.
- keyfile: Optional argument that specifies the path to the file containing the encryption key.

Some common actions of the cryptsetup command are:

- luksFormat: This action encrypts the specified device with LUKS (Linux Unified Key Setup), which is a standard for disk encryption in Linux. It prompts the user to set a passphrase, which will be required to unlock the encrypted device in the future.

Example: 
```
cryptsetup luksFormat /dev/sda1
```

- luksOpen: This action unlocks and opens the encrypted device, so that it can be accessed like an unencrypted volume.

Example: 
```
cryptsetup luksOpen /dev/sda1 my_encrypted_volume
```

- resize: This action resizes an encrypted device, without affecting the data inside.

Example:
```
cryptsetup resize my_encrypted_volume
```

- luksClose: This action closes the encrypted device and removes it from the system.

Example: 
```
cryptsetup luksClose my_encrypted_volume
```

Other options of the cryptsetup command include:
- --batch-mode: Runs the command in non-interactive mode, useful when automating encryption tasks.
- --verify-passphrase: Prompts the user to verify the entered passphrase, to avoid typos or mistakes.
- --key-size: Specifies the size of the encryption key, in bits.
- --hash: Specifies the type of hash function to use for generating the encryption key.
- --iter-time: Specifies the number of iterations for the key derivation function, which affects the strength of the encryption. 

## tldr 
 
> Manage plain dm-crypt and LUKS (Linux Unified Key Setup) encrypted volumes.
> More information: <https://gitlab.com/cryptsetup/cryptsetup/>.

- Initialize a LUKS volume (overwrites all data on the partition):

`cryptsetup luksFormat {{/dev/sda1}}`

- Open a LUKS volume and create a decrypted mapping at `/dev/mapper/{{target}}`:

`cryptsetup luksOpen {{/dev/sda1}} {{target}}`

- Remove an existing mapping:

`cryptsetup luksClose {{target}}`

- Change the LUKS volume's passphrase:

`cryptsetup luksChangeKey {{/dev/sda1}}`
