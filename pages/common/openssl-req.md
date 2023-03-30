# openssl req 
## chatgpt 
OpenSSL is an open-source cryptographic software library that provides a series of tools for secure communication and data encryption. The "req" command is one of the commands in the OpenSSL library that generates a new certificate signing request (CSR).

A CSR contains information about the entity (person or organization) that is requesting a digital certificate, such as the domain name, the public key, and the information about the organization. It is used to request a digital certificate from a Certificate Authority (CA), which subsequently issues a digital certificate to the requester.

The "openssl req" command has specific parameters that need to be included in the command to generate a CSR. The different parameters used in the command include:

1) "-newkey": This parameter creates a new private key and the algorithm used to generate the key. For example, "-newkey rsa:2048" creates a 2048-bit RSA key.

2) "-keyout": This parameter specifies the file name and directory where the newly generated private key will be stored.

3) "-out": This parameter specifies the file name and directory where the CSR will be stored.

4) "-subj": This parameter allows the user to specify the subject DN (Distinguished Name) of the CSR. The DN consists of several pieces of information, such as the name, organization, country code, state or province, and locality.

By using all these parameters, the "openssl req" command generates a new CSR, which can be used to request a digital certificate from a CA. 

## tldr 
 
> OpenSSL command to manage PKCS#10 Certificate Signing Requests.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-req.html>.

- Generate a certificate signing request to be sent to a certificate authority:

`openssl req -new -sha256 -key {{filename.key}} -out {{filename.csr}}`

- Generate a self-signed certificate and a corresponding key-pair, storing both in a file:

`openssl req -new -x509 -newkey {{rsa}}:{{4096}} -keyout {{filename.key}} -out {{filename.cert}} -subj "{{/C=XX/CN=foobar}}" -days {{365}}`
