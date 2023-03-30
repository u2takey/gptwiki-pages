# gmssl 
## chatgpt 
`gmssl` is a command-line tool for OpenSSL-compatible cryptographic functions and protocols, developed by Guomi Digital Technology Co. Ltd. It provides various functions such as encryption, decryption, digital signature generation and verification, and key management. The command can perform various cryptographic operations using different algorithms such as SM2, SM3, SM4, and RSA. 

Here are some of the common functions that can be performed using `gmssl`:

- Generating a public/private key pair: `gmssl genpkey -algorithm SM2 -out sm2.key`
- Creating a digital signature: `gmssl dgst -sign sm2.key -keyform PEM -sm3 file.txt > file.sig`
- Verifying a digital signature: `gmssl dgst -verify pubkey.pem -keyform PEM -sm3 -signature file.sig file.txt`
- Encrypting a file using SM4: `gmssl enc -SM4-CBC -in plaintext.txt -out ciphertext.txt -K 1234567890123456 -iv 1234567890123456`
- Decrypting a file using SM4: `gmssl enc -d -SM4-CBC -in ciphertext.txt -out plaintext.txt -K 1234567890123456 -iv 1234567890123456`

Overall, `gmssl` provides a powerful set of cryptographic functions that can be used to secure data, generate digital signatures, and manage keys. It is widely used in China and other countries where SM2 and other Chinese cryptographic standards are required. 

## tldr 
 
> GmSSL is a crypto toolkit supporting SM1, SM2, SM3, SM4, SM9, and ZUC/ZUC256.
> More information: <http://gmssl.org/english.html>.

- Generate an SM3 hash for a file:

`gmssl sm3 {{path/to/file}}`

- Encrypt a file using the SM4 cipher:

`gmssl sms4 -e -in {{path/to/file}} -out {{path/to/file.sms4}}`

- Decrypt a file using the SM4 cipher:

`gmssl sms4 -d -in {{path/to/file.sms4}}`

- Generate an SM2 private key:

`gmssl sm2 -genkey -out {{path/to/file.pem}}`

- Generate an SM2 public key from an existing private key:

`gmssl sm2 -pubout -in {{path/to/file.pem}} -out {{path/to/file.pem.pub}}`

- Encrypt a file using the ZUC cipher:

`gmssl zuc -e -in {{path/to/file}} -out {{path/to/file.zuc}}`

- Decrypt a file using the ZUC cipher:

`gmssl zuc -d -in {{path/to/file.zuc}}`

- Print version:

`gmssl version`
