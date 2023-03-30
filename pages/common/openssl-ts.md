# openssl ts 
## chatgpt 
The `openssl ts` command is used to generate and verify timestamps using the Time Stamp Protocol (TSP). TSP is a protocol for certifying the existence of a certain document or data at a certain time. It is used for ensuring document authenticity and preventing unauthorized modification.

The command can be used with various options depending on the desired operation. Some of the options are:

- `-query`: This option is used to generate a timestamp query for a specific data or file.
- `-reply`: This option is used to verify a timestamp response against the initial data or file.
- `-policy`: This option is used to specify the policy OID (object identifier) for timestamping.
- `-cert`: This option is used to specify the certificate file to be used for timestamping.

The exact usage of the `openssl ts` command can vary based on the specific use case and options used. 

## tldr 
 
> OpenSSL command to generate and verify timestamps.
> More information: <https://www.openssl.org/docs/manmaster/man1/openssl-ts.html>.

- Generate a SHA-512 timestamp request of a specific file and output to `file.tsq`:

`openssl ts -query -data {{path/to/file}} -sha512 -out {{path/to/file.tsq}}`

- Check the date and metadata of a specific timestamp response file:

`openssl ts -reply -in {{path/to/file.tsr}} -text`

- Verify a timestamp request file and a timestamp response file from the server with an SSL certificate file:

`openssl ts -verify -in {{path/to/file.tsr}} -queryfile {{path/to/file.tsq}} -partial_chain -CAfile {{path/to/cert.pem}}`

- Create a timestamp response for request using key and signing certificate and output it to `file.tsr`:

`openssl ts -reply -queryfile {{path/to/file.tsq}} -inkey {{path/to/tsakey.pem}} -signer tsacert.pem -out {{path/to/file.tsr}}`
