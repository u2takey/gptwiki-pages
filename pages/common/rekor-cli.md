# rekor-cli 
## chatgpt 
The `rekor-cli` command is a command-line tool for interacting with the Rekor transparency log, which is a tamper-evident, append-only log of software transparency data. The Rekor project is an open-source project that provides a way to track metadata about software artifacts, such as code signing certificates, cryptographic hashes, and provenance information.

The `rekor-cli` command provides various subcommands for interacting with the Rekor transparency log, such as:

- `log`: Allows users to record transparency data in the Rekor log.
- `get`: Allows users to retrieve transparency data from the Rekor log.
- `prove`: Allows users to generate a cryptographic proof that a given piece of data is in the Rekor log.
- `verify`: Allows users to verify a previously generated proof that a given piece of data is in the Rekor log.
- `key`: Allows users to manage cryptographic keys for interacting with the Rekor transparency log.

The `rekor-cli` command is useful for developers and security professionals who want to ensure the integrity and provenance of software artifacts, as well as for organizations that want to ensure compliance with industry regulations and best practices. 

## tldr 
 
> Immutable tamper resistant ledger of metadata generated within a software projects supply chain.
> More information: <https://github.com/sigstore/rekor>.

- Upload an artifact to Rekor:

`rekor-cli upload --artifact {{path/to/file.ext}} --signature {{path/to/file.ext.sig}} --pki-format={{x509}} --public-key={{path/to/key.pub}}`

- Get information regarding entries in the Transparency Log:

`rekor-cli get --uuid={{0e81b4d9299e2609e45b5c453a4c0e7820ac74e02c4935a8b830d104632fd2d1}}`

- Search the Rekor index to find entries by Artifact:

`rekor-cli search --artifact {{path/to/file.ext}}`

- Search the Rekor index to find entries by a specific hash:

`rekor-cli search --sha {{6b86b273ff34fce19d6b804eff5a3f5747ada4eaa22f1d49c01e52ddb7875b4b}}`
