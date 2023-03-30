# certutil 
## chatgpt 
Certutil is a command-line utility in Windows that is used to manage and configure certificates and certificate stores on a Windows computer. Certificates are used for secure communication between computers.

The certutil command can be used to perform a variety of operations, including:

1. Importing and Exporting Certificates: Certificates can be imported and exported using the certutil command. This is useful when migrating certificates from one computer to another.

2. Managing Certificates: Certutil can be used to manage certificates, including adding and removing certificates, setting properties, and configuring trust options.

3. Testing Certificates: Certutil can be used to test certificates to ensure they are valid and functioning properly.

4. Viewing Certificate Information: Certutil can be used to view certificate information, including certificate details, certificate chain information, and certificate revocation lists (CRLs).

5. Creating Certificate Requests: Certutil can be used to create a certificate request, which is used to request a new certificate from a certificate authority (CA).

The certutil command is used with various switches and parameters to perform these operations. The syntax for the command is:

certutil [options] [arguments]

Some common options that can be used with the certutil command include:

- -import: Imports a certificate into a certificate store.

- -viewstore: Views the contents of a certificate store.

- -addstore: Adds a certificate to a certificate store.

- -delstore: Deletes a certificate from a certificate store.

- -verify: Verifies the validity of a certificate.

- -ping: Checks to see if a certificate authority is responding.

Overall, certutil is a powerful command-line tool that allows administrators to manage and configure certificates for secure communication in Windows environments. 

## tldr 
 
> Manage keys and certificates in both NSS databases and other NSS tokens.
> More information: <https://manned.org/certutil>.

- Create a new certificate database:

`certutil -N -d .`

- List all certificates in a database:

`certutil -L -d .`

- List all private keys in a database:

`certutil -K -d . -f {{path/to/password_file.txt}}`

- Import the signed certificate into the requesters database:

`certutil -A -n "{{server_certificate}}" -t ",," -i {{path/to/file.crt}} -d .`

- Add subject alternative names to a given certificate:

`certutil -S -f {{path/to/password_file.txt}} -d . -t ",," -c "{{server_certificate}}" -n "{{server_name}}" -g {{2048}} -s "CN={{common_name}},O={{organization}}"`
