# openssl dgst 
## chatgpt 
The command "openssl dgst" is used for generating the message digest of a given file using a hash function algorithm. It is a part of the OpenSSL suite, which is an open-source software library that provides SSL and TLS protocols for secure communication over the internet.

The syntax for the "openssl dgst" command is:

openssl dgst [-md5 | -sha1 | -sha256 | -sha384 | -sha512 | ...] [input_file]

Here, the "[-md5 | -sha1 | -sha256 | -sha384 | -sha512 | ...]" argument specifies the hash function algorithm to be used for generating the message digest. The available hash algorithms depending upon the version of OpenSSL installed on your system.

The "input_file" argument specifies the file for which the message digest needs to be generated. If this argument is not specified, the "openssl dgst" command reads from the standard input.

Once you enter the command, OpenSSL calculates the hash of the input file and displays the output to the terminal. The output contains the hash value, followed by the name of the file.

You can use the "openssl dgst" command for various purposes, such as generating checksums, verifying file integrity, and detecting data tampering. 

## tldr 
 
> OpenSSL command to generate digest values and perform signature operations.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-dgst.html>.

- Calculate the SHA256 digest for a file, saving the result to a specific file:

`openssl dgst -sha256 -binary -out {{output_file}} {{input_file}}`

- Sign a file using an RSA key, saving the result to a specific file:

`openssl dgst -sign {{private_key_file}} -sha256 -sigopt rsa_padding_mode:pss -out {{output_file}} {{input_file}}`

- Verify an RSA signature:

`openssl dgst -verify {{public_key_file}} -signature {{signature_file}} -sigopt rsa_padding_mode:pss {{signature_message_file}}`

- Sign a file using and ECDSA key:

`openssl dgst -sign {{private_key_file}} -sha256 -out {{output_file}} {{input_file}}`

- Verify an ECDSA signature:

`openssl dgst -verify {{public_key_file}} -signature {{signature_file}} {{signature_message_file}}`
