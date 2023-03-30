# hardhat 
## chatgpt 
Hardhat is a development environment for building and testing smart contracts on the Ethereum blockchain. It provides a number of tools and features that make it easier for developers to write, test, and deploy smart contracts. Some of the key features and tools include:

1. Smart Contract Development: Hardhat provides a built-in console for interacting with smart contracts, as well as a suite of development tools for testing and debugging.

2. Test Networks: Hardhat comes with pre-configured local networks that allow developers to test their smart contracts in a simulated environment before deploying them to the main network.

3. Plugin Architecture: Hardhat has a plugin architecture that allows developers to extend its functionality with additional tools and features.

4. Automated Testing: Hardhat provides an automated testing framework that makes it easy to write and run tests for smart contracts.

5. Ethereum Mainnet Deployment: Hardhat provides a streamlined deployment process for deploying smart contracts to the Ethereum mainnet.

Overall, Hardhat is a powerful tool for Ethereum developers that simplifies smart contract development and testing, while also providing a range of advanced features for deploying contracts to the blockchain. 

## tldr 
 
> A development environment for Ethereum software.
> More information: <https://hardhat.org>.

- List available subcommands (or create a new project if no configuration exists):

`hardhat`

- Compile the current project and build all artifacts:

`hardhat compile`

- Run a user-defined script after compiling the project:

`hardhat run {{path/to/script.js}}`

- Run Mocha tests:

`hardhat test`

- Run all given test files:

`hardhat test {{path/to/file1.js}} {{path/to/file2.js}}`

- Start a local Ethereum JSON-RPC node for development:

`hardhat node`

- Start a local Ethereum JSON-RPC node with a specific hostname and port:

`hardhat node --hostname {{hostname}} --port {{port}}`

- Clean the cache and all artifacts:

`hardhat clean`
