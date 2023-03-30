# cipher 
## chatgpt 
The cipher command in Windows is used to encrypt or decrypt files and folders on a specific drive or directory. It uses an encryption algorithm called Advanced Encryption Standard (AES) to protect data.

The syntax for using the cipher command is:

cipher [/E | /D] [/S:directory] [/A] [/I] [/F] [/Q] [/H] [/K] [pathname [...]]

- /E - Encrypts the specified files or directories.
- /D - Decrypts the specified files or directories.
- /S - Operates on files in the specified directory and all subdirectories.
- /A - Indicates that files with the archive attribute should be encrypted or decrypted.
- /I - Ignores errors during the encryption or decryption process.
- /F - Forces the encryption or decryption of files, even if there are errors.
- /Q - Enables Quiet mode, which suppresses the display of encryption or decryption status.
- /H - Displays files with hidden or system attributes.
- /K - Creates a new file encryption key.

When you run the cipher command without any arguments, it displays the current encryption status of the files and directories in the current directory.

Warning: Using the cipher command to encrypt files does not guarantee their security. It is recommended to use additional methods, such as using a strong password and storing the files on a secure drive, to ensure that confidential information is protected. 

## tldr 
 
> Display or alter the encryption of directories and files on NTFS volumes.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/cipher>.

- Display information about a specific encrypted file or directory:

`cipher /c:{{path\to\file_or_directory}}`

- [e]ncrypt a file or directory (files added later to the directory are also encrypted as the directory is marked):

`cipher /e:{{path\to\file_or_directory}}`

- [d]ecrypt a file or directory:

`cipher /d:{{path\to\file_or_directory}}`

- Securely remove a file or directory:

`cipher /w:{{path\to\file_or_directory}}`
