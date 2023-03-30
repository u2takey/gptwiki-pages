# keybase 
## chatgpt 
`keybase` is a command-line tool that is used for secure messaging, file sharing, and identity verification. It is used to verify the identity of users using their social media accounts like Twitter, Facebook, and GitHub. 

Some of the main functions of the `keybase` command are:

- To create a new Keybase account
- To verify your social media accounts 
- To encrypt and decrypt messages
- To share files securely with other Keybase users
- To sign and verify messages 
- To manage your Keybase identity 

To use the `keybase` command, you need to have it installed on your system. Once installed, you can open a terminal and type `keybase` followed by the specific subcommand you wish to use. For example, `keybase login` will allow you to log into your existing Keybase account, while `keybase encrypt` will allow you to encrypt a message for another user. 

Overall, the `keybase` command is a powerful tool for secure communication and identity verification. It is an excellent option for users who want to keep their online activity private and secure. 

## tldr 
 
> Key directory that maps social media identities to encryption keys in a publicly auditable manner.
> More information: <https://keybase.io/docs/command_line>.

- Follow another user:

`keybase follow {{username}}`

- Add a new proof:

`keybase prove {{service}} {{service_username}}`

- Sign a file:

`keybase sign --infile {{input_file}} --outfile {{output_file}}`

- Verify a signed file:

`keybase verify --infile {{input_file}} --outfile {{output_file}}`

- Encrypt a file:

`keybase encrypt --infile {{input_file}} --outfile {{output_file}} {{receiver}}`

- Decrypt a file:

`keybase decrypt --infile {{input_file}} --outfile {{output_file}}`

- Revoke current device, log out, and delete local data:

`keybase deprovision`
