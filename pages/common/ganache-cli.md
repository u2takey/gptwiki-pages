# ganache-cli 
## chatgpt 
ganache-cli is a command-line tool used for running local Ethereum blockchain networks for development and testing purposes. 

When you run the command ganache-cli, it initializes a local blockchain network with 10 accounts loaded with 100 fake Ether each, allowing developers to quickly and easily test smart contracts and DApps locally without needing to deploy them to the main Ethereum network. 

The ganache-cli command provides a wide range of options to configure the network parameters, such as setting gas limits, block times, network id, and more. Users can also use ganache-cli to create custom accounts with specific Ether balances, private keys, and other parameters for testing.

ganache-cli also provides a CLI interface to interact with the local network and to inspect the state of the blockchain, including balances, smart contract code, and transaction messages. It also supports integration with popular development frameworks such as Truffle and Web3.js, making it a valuable tool for Ethereum developers. 

## tldr 
 
> Command-line version of Ganache, your personal blockchain for Ethereum development.
> More information: <https://www.trufflesuite.com/ganache>.

- Run Ganache:

`ganache-cli`

- Run Ganache with a specific number of accounts:

`ganache-cli --accounts={{number_of_accounts}}`

- Run Ganache and lock available accounts by default:

`ganache-cli --secure`

- Run Ganache server and unlock specific accounts:

`ganache-cli --secure --unlock "{{account_private_key1}}" --unlock "{{account_private_key2}}"`

- Run Ganache with a specific account and balance:

`ganache-cli --account="{{account_private_key}},{{account_balance}}"`

- Run Ganache with accounts with a default balance:

`ganache-cli --defaultBalanceEther={{default_balance}}`

- Run Ganache and log all requests to `stdout`:

`ganache-cli --verbose`
