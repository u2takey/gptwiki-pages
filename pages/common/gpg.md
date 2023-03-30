# gpg 
## chatgpt 
The "gpg" command stands for GNU Privacy Guard, which is a free and open-source implementation of the OpenPGP standard to encrypt and sign data.

The "gpg" command is used in a command-line interface (CLI) to perform various operations related to GnuPG, such as generating and managing encryption keys, encrypting and decrypting files and messages, verifying signatures, and so on.

Here are some of the most common operations you can perform with the "gpg" command:

- Generating a new encryption key: `gpg --gen-key`
- Listing existing keys: `gpg --list-keys`
- Encrypting a file or message: `gpg -e -r recipient file.txt`
- Decrypting a file or message: `gpg -d file.gpg`
- Signing a file or message: `gpg --sign file.txt`
- Verifying a signature: `gpg --verify file.txt.sig`

The "gpg" command is a powerful tool for securing your data and communications, but it requires some knowledge and expertise to manage encryption keys, verify signatures, and use it effectively. It is recommended to read the GnuPG documentation and tutorials to learn how to use it properly. 

## tldr 
 
> GNU Privacy Guard.
> See `gpg2` for GNU Privacy Guard 2. Most operating systems symlink `gpg` to `gpg2`.
> More information: <https://gnupg.org>.

- Create a GPG public and private key interactively:

`gpg --full-generate-key`

- Sign `doc.txt` without encryption (writes output to `doc.txt.asc`):

`gpg --clearsign {{doc.txt}}`

- Encrypt and sign `doc.txt` for alice@example.com and bob@example.com (output to `doc.txt.gpg`):

`gpg --encrypt --sign --recipient {{alice@example.com}} --recipient {{bob@example.com}} {{doc.txt}}`

- Encrypt `doc.txt` with only a passphrase (output to `doc.txt.gpg`):

`gpg --symmetric {{doc.txt}}`

- Decrypt `doc.txt.gpg` (output to `stdout`):

`gpg --decrypt {{doc.txt.gpg}}`

- Import a public key:

`gpg --import {{public.gpg}}`

- Export public key for alice@example.com (output to `stdout`):

`gpg --export --armor {{alice@example.com}}`

- Export private key for alice@example.com (output to `stdout`):

`gpg --export-secret-keys --armor {{alice@example.com}}`
