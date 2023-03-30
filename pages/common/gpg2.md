# gpg2 
## chatgpt 
gpg2 is a command-line tool used for encryption and digital signature operations on files and communication channels. The "gpg" in gpg2 stands for GnuPG, which is short for GNU Privacy Guard. 

The tool is used to encrypt sensitive files and data so that they cannot be read by unauthorized persons. It uses a public key infrastructure to encrypt and decrypt data. The user generates a pair of encryption keys, a private key that is kept secret and a public key that can be shared freely. The public key is used to encrypt files before being sent to the recipient who then decrypts it using their own private key.

In addition to encryption and decryption, gpg2 is also used to sign digital documents and verify the signature of received documents. This provides integrity and authenticity in electronic communication.

Overall, gpg2 is a powerful tool for ensuring the confidentiality, integrity, and authenticity of electronic communication and data. 

## tldr 
 
> GNU Privacy Guard 2.
> See `gpg` for GNU Privacy Guard 1.
> More information: <https://docs.releng.linuxfoundation.org/en/latest/gpg.html>.

- List imported keys:

`gpg2 --list-keys`

- Encrypt a specified file for a specified recipient, writing the output to a new file with `.gpg` appended:

`gpg2 --encrypt --recipient {{alice@example.com}} {{path/to/doc.txt}}`

- Encrypt a specified file with only a passphrase, writing the output to a new file with `.gpg` appended:

`gpg2 --symmetric {{path/to/doc.txt}}`

- Decrypt a specified file, writing the result to the standard output:

`gpg2 --decrypt {{path/to/doc.txt.gpg}}`

- Import a public key:

`gpg2 --import {{path/to/public_key.gpg}}`

- Export the public key of a specified email address to the standard output:

`gpg2 --export --armor {{alice@example.com}}`

- Export the private key with a specified email address to the standard output:

`gpg2 --export-secret-keys --armor {{alice@example.com}}`
