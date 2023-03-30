# ipfs 
## chatgpt 
IPFS stands for InterPlanetary File System, which is a peer-to-peer distributed network protocol that provides a platform for creating a decentralized storage and sharing network. IPFS enables users to store and access files in a decentralized manner, making it a powerful tool for building a distributed web.

The command "ipfs" is the entry point for interacting with the IPFS system from the command line. It is a useful tool for performing various tasks such as adding content to the network, retrieving content from the network, searching for content, and managing nodes in the network.

Some of the most commonly used subcommands for IPFS are:

- "ipfs add" - to add files to the IPFS network.
- "ipfs cat" - to retrieve content from the network.
- "ipfs ls" - to list the contents of a specific IPFS object or directory.
- "ipfs pin" - to pin content to ensure it is persistently available on the network.
- "ipfs swarm" - to manage network peers and connections.
- "ipfs id" - to retrieve information about your own node, including your peer ID, protocol version, and public key.

Overall, the "ipfs" command provides a convenient and powerful interface for interacting with the IPFS network and leveraging the benefits of decentralized storage and sharing. 

## tldr 
 
> Inter Planetary File System.
> A peer-to-peer hypermedia protocol. Aims to make the web more open.
> More information: <https://ipfs.io>.

- Add a file from local to the filesystem, pin it and print the relative hash:

`ipfs add {{path/to/file}}`

- Add a directory and its files recursively from local to the filesystem and print the relative hash:

`ipfs add -r {{path/to/directory}}`

- Save a remote file and give it a name but not pin it:

`ipfs get {{hash}} -o {{path/to/file}}`

- Pin a remote file locally:

`ipfs pin add {{hash}}`

- Display pinned files:

`ipfs pin ls`

- Unpin a file from the local storage:

`ipfs pin rm {{hash}}`

- Remove unpinned files from local storage:

`ipfs repo gc`
