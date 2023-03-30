# electrum 
## chatgpt 
Electrum is a command-line cryptocurrency wallet application that is primarily used to manage Bitcoin. The command "electrum" launches the Electrum application, which can be used to perform a variety of functions related to Bitcoin management.

When the "electrum" command is executed, it launches the Electrum application and presents the user with a login screen. If the user already has an existing Electrum wallet, they can enter their wallet seed or private keys to access their funds. If the user does not have an existing wallet, they can create a new one by following the on-screen instructions.

Once the user has logged in, they can use the Electrum application to send and receive Bitcoin, view their transaction history, manage their addresses, set transaction fees, and perform other operations related to Bitcoin. The Electrum application also includes advanced features such as support for multi-signature transactions and integration with hardware wallets.

Overall, the "electrum" command is a versatile tool for managing Bitcoin and provides a user-friendly interface for performing a variety of functions related to Bitcoin management. 

## tldr 
 
> Ergonomic Bitcoin wallet and private key management.
> More information: <https://electrum.org>.

- Create a new wallet:

`electrum -w {{new_wallet.dat}} create`

- Restore an existing wallet from seed offline:

`electrum -w {{recovery_wallet.dat}} restore -o`

- Create a signed transaction offline:

`electrum mktx {{recipient}} {{amount}} -f 0.0000001 -F {{from}} -o`

- Display all wallet receiving addresses:

`electrum listaddresses -a`

- Sign a message:

`electrum signmessage {{address}} {{message}}`

- Verify a message:

`electrum verifymessage {{address}} {{signature}} {{message}}`

- Connect only to a specific electrum-server instance:

`electrum -p socks5:{{127.0.0.1}}:9050 -s {{56ckl5obj37gypcu.onion}}:50001:t -1`
