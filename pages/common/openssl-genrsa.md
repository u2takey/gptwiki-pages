# openssl genrsa 
## chatgpt 
The 'openssl genrsa' command is used to generate an RSA (Rivest-Shamir-Adleman) private key. RSA is a widely used public-key cryptography algorithm that is used for secure data transmission and is based on the difficulty of factoring large integers.

The 'genrsa' sub-command generates a private key using the RSA algorithm. It takes in options such as the key size (-out filename), the encryption algorithm to use (-aes128), and more. If no options are specified, a default key size of 2048 bits is generated.

The output of the command is a PEM (Privacy Enhanced Mail) format file containing the generated private key. This PEM file can be used in SSL/TLS certificates, SSH connectivity, encrypting/decrypting files, and other secure communications applications.

Overall, openssl genrsa command is an important tool for generating secure private keys for applications that require secure communications. 

## tldr 
 
> OpenSSL command to generate RSA private keys.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-genrsa.html>.

- Generate an RSA private key of 2048 bits to `stdout`:

`openssl genrsa`

- Save an RSA private key of an arbitrary number of bits to the output file:

`openssl genrsa -out {{output_file.key}} {{1234}}`

- Generate an RSA private key and encrypt it with AES256 (you will be prompted for a passphrase):

`openssl genrsa {{-aes256}}`
