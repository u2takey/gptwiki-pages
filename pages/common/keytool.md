# keytool 
## chatgpt 
Keytool is a utility tool provided by Java that allows a user to manage digital certificates and cryptographic keys.

The "keytool" command can be used to perform various cryptographic operations such as generating a new key pair, creating and managing key store files, importing and exporting digital certificates, and printing certificate information.

Below are some of the commonly used options with the keytool command:

1. -genkeypair: This option is used to generate a new key pair and stores it in a key store file.

2. -list: This option is used to list the certificates and keys stored in a key store file.

3. -import: This option is used to import a certificate from a file into a key store file.

4. -export: This option is used to export a certificate from a key store file.

5. -delete: This option is used to delete a certificate or key from a key store file.

Overall, the keytool command is a powerful tool for managing digital certificates and cryptographic keys in Java applications. 

## tldr 
 
> Keytool is a certificate management utility included with Java.
> More information: <https://docs.oracle.com/en/java/javase/19/docs/specs/man/keytool.html>.

- Create a keystore:

`keytool -genkeypair -v -keystore {{path/to/file.keystore}} -alias {{key_name}}`

- Change a keystore password:

`keytool -storepasswd -keystore {{path/to/file.keystore}}`

- Change a key's password inside a specific keystore:

`keytool -keypasswd  -alias {{key_name}} -keystore {{path/to/file.keystore}}`
