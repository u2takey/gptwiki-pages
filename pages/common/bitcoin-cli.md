# bitcoin-cli 
## chatgpt 
"bitcoin-cli" is a command-line interface (CLI) provided by the Bitcoin Core software. It allows users to interact with a Bitcoin node via the command line interface by sending RPC (Remote Procedure Call) requests to the node. 

Bitcoin-cli can be used to perform various functions, including managing accounts, sending and receiving payments, viewing the blockchain, generating private keys, and much more. 

To use bitcoin-cli, you need to have a running Bitcoin node on your computer with the corresponding rpcuser and rpcpassword. You can then invoke bitcoin-cli and pass parameters to execute a command. For example, to get the balance of a Bitcoin address, you would execute the following command:

bitcoin-cli getbalance <bitcoin_address>

This command sends an RPC request to the Bitcoin node to get the balance of a given Bitcoin address. The result will be displayed on the command line interface.

Overall, bitcoin-cli is a powerful tool for managing a Bitcoin node and performing various tasks related to Bitcoin. However, it should be used with caution, as incorrect commands could result in irreversible financial losses. 

## tldr 
 
> Command-line client to interact with the Bitcoin daemon via RPC calls.
> Uses the configuration defined in `bitcoin.conf`.
> More information: <https://en.bitcoin.it/wiki/Running_Bitcoin#Command-line_arguments>.

- Send a transaction to a given address:

`bitcoin-cli sendtoaddress "{{address}}" {{amount}}`

- Generate one or more blocks:

`bitcoin-cli generate {{num_blocks}}`

- Print high-level information about the wallet:

`bitcoin-cli getwalletinfo`

- List all outputs from previous transactions available to fund outgoing transactions:

`bitcoin-cli listunspent`

- Export the wallet information to a text file:

`bitcoin-cli dumpwallet "{{path/to/file}}"`
