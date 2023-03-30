# minisign 
## chatgpt 
Minisign is a command-line tool used for signing and verifying files. It uses public-key cryptography to create digital signatures that can verify the integrity and authenticity of a file. 

When signing a file with minisign, the user generates a public/private key pair. The private key is kept secret and used to sign files, while the public key can be freely distributed. The person receiving the signed file can then use the signer's public key to verify the signature and ensure that the file has not been modified since it was signed.

The basic syntax for the minisign command is as follows:

minisign -Sm <file-to-sign> -s <keyfile>

The -Sm option specifies that the file should be signed and hashed using BLAKE2b. The -s option specifies the location of the private key file to use for signing.

To verify a signed file, the basic syntax is:

minisign -Vm <signed-file> -p <public-key>

The -Vm option specifies that the file should be verified, and the -p option specifies the location of the public key file to use for verification.

Overall, minisign is a simple yet powerful tool for ensuring the authenticity and integrity of files, and is often used in situations where security is of the utmost importance, such as in software development and distribution. 

## tldr 
 
> A dead simple tool to sign files and verify signatures.
> More information: <https://jedisct1.github.io/minisign/>.

- Generate a new keypair at the default location:

`minisign -G`

- Sign a file:

`minisign -Sm {{path/to/file}}`

- Sign a file, adding a trusted (signed) and an untrusted (unsigned) comment in the signature:

`minisign -Sm {{path/to/file}} -c "{{Untrusted comment}}" -t "{{Trusted comment}}"`

- Verify a file and the trusted comments in its signature using the specified public key file:

`minisign -Vm {{path/to/file}} -p {{path/to/publickey.pub}}`

- Verify a file and the trusted comments in its signature, specifying a public key as a Base64 encoded literal:

`minisign -Vm {{path/to/file}} -P "{{public_key_base64}}"`
