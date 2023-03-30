# hsd-cli 
## chatgpt 
The `hsd-cli` command refers to the command-line interface for the Handshake node software (HSD). Handshake is a decentralized, open-source blockchain platform that provides a decentralized domain name registry service.

The `hsd-cli` command allows users to interact with the Handshake node via a command-line interface (CLI). It provides various functionalities, including querying wallet and blockchain information, sending transactions, creating and managing wallets, accessing API endpoints, and more.

The `hsd-cli` command requires users to have a Handshake node running on their machine, and they can interact with the node by using the command's syntax and arguments.

Some common `hsd-cli` commands include:
- `hsd-cli getbalance`: This command retrieves the balance of the specified wallet.
- `hsd-cli sendtoaddress`: This command sends a specified amount of Handshake coins to the specified address.
- `hsd-cli generate`: This command generates new blocks on the Handshake network.
- `hsd-cli createnewwallet`: This command creates a new Handshake wallet and generates a new address to receive coins.

Overall, the `hsd-cli` command is a powerful tool for developers and advanced users who want to interact with the Handshake network and build on top of it. 

## tldr 
 
> The command-line REST tool for the Handshake blockchain.
> More information: <https://handshake.org>.

- Retrieve information about the current server:

`hsd-cli info`

- Broadcast a local transaction:

`hsd-cli broadcast {{transaction_hex}}`

- Retrieve a mempool snapshot:

`hsd-cli mempool`

- View a transaction by address or hash:

`hsd-cli tx {{address_or_hash}}`

- View a coin by its hash index or address:

`hsd-cli coin {{hash_index_or_address}}`

- View a block by height or hash:

`hsd-cli block {{height_or_hash}}`

- Reset the chain to the specified block:

`hsd-cli reset {{height_or_hash}}`

- Execute an RPC command:

`hsd-cli rpc {{command}} {{args}}`
