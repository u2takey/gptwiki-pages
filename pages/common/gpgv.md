# gpgv 
## chatgpt 
The gpgv command is a tool used to check the integrity of OpenPGP signatures on files. It is often used in conjunction with GnuPG (GPG), a free and open-source encryption software suite.

The syntax of the gpgv command is as follows:

gpgv [options] file

Where "file" is the name of the file containing the signature to be verified.

Some common options for the gpgv command include:

- -v, which enables verbose output
- -q, which suppresses output
- -i, which specifies an additional keyring to use for verification
- -k, which prints a list of trusted keys

The gpgv command works by verifying the signature of a file using a trusted key. The signature itself is created by the sender of the file using their private key, and the recipient can use the sender's public key to verify that the signature is valid.

During verification, gpgv checks that the signature is valid, that it was created by the expected sender, and that the file has not been modified since it was signed. If the signature is invalid, gpgv will report an error.

Overall, the gpgv command is an important tool for verifying the authenticity and integrity of files that have been digitally signed using OpenPGP. 

## tldr 
 
> Verify OpenPGP signatures.
> More information: <https://www.gnupg.org/documentation/manuals/gnupg/gpgv.html>.

- Verify a signed file:

`gpgv {{path/to/file}}`

- Verify a signed file using a detached signature:

`gpgv {{path/to/signature}} {{path/to/file}}`

- Add a file to the list of keyrings (a single exported key also counts as a keyring):

`gpgv --keyring {{./alice.keyring}} {{path/to/signature}} {{path/to/file}}`
