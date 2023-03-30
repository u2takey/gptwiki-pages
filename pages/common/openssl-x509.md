# openssl x509 
## chatgpt 
The command "openssl x509" is a Linux command that is used to display and manage X.509 certificates. Here's a detailed explanation of the command:

- openssl: It is the command for the OpenSSL toolkit which is a software library that provides a secure communication layer over networks. It is used to implement secure communication protocols like HTTPS, SSH, and SSL/TLS.

- x509: It is the subcommand of the openssl command used to work with X.509 certificates.

X.509 is a standard that defines the format of public key certificates that are used in SSL/TSL encrypted connections. X.509 certificates contain information about the identity of the certificate holder, the certificate issuing authority, and the validity period of the certificate.

The openssl x509 command can be used to perform the following operations:

1. Display certificate details: The command can be used to display the details of a certificate like the subject name, issuer name, serial number, public key, certificate expiry date, etc.

2. Convert certificate formats: The command can be used to convert a certificate from one format to another, like from PEM to DER, or vice versa.

3. Verify certificate: The command can be used to verify the integrity of a certificate by checking its digital signature against the public key of the issuing authority.

4. Extract public key: The command can be used to extract the public key from a certificate which can be used for encryption or digital signature verification.

Overall, the "openssl x509" command is a powerful tool for managing X.509 certificates in Linux systems. 

## tldr 
 
> OpenSSL command to manage X.509 certificates.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-x509.html>.

- Display certificate information:

`openssl x509 -in {{filename.crt}} -noout -text`

- Display a certificate's expiration date:

`openssl x509 -enddate -noout -in {{filename.pem}}`

- Convert a certificate between binary DER encoding and textual PEM encoding:

`openssl x509 -inform {{der}} -outform {{pem}} -in {{original_certificate_file}} -out {{converted_certificate_file}}`

- Store a certificate's public key in a file:

`openssl x509 -in {{certificate_file}} -noout -pubkey -out {{output_file}}`
