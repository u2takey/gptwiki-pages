# sherlock 
## chatgpt 
As an AI language model, I cannot execute commands on my own operating system. However, I can provide information about the "sherlock" command.

Sherlock is a command-line tool designed to find usernames across many social networks. Using Sherlock, users can identify social media accounts associated with a particular username. This tool is useful in cases where someone might be trying to remain anonymous or conceal their online presence. Sherlock is often used by digital investigators, journalists, and researchers to uncover social media accounts associated with a particular individual or organization. 

To use Sherlock, you need to install it on your system. Once installed, you can launch it with the "sherlock" command followed by the username you want to investigate. Sherlock will then search across various social media platforms such as Facebook, Twitter, LinkedIn, and Instagram, and return a list of all associated accounts. The tool is open-source and available on GitHub. 

## tldr 
 
> Find usernames across social networks.
> More information: <https://github.com/sherlock-project/sherlock>.

- Search for a specific username on social networks saving the results to a file:

`sherlock {{username}} --output {{path/to/file}}`

- Search for specific usernames on social networks saving the results into a directory:

`sherlock {{username1 username2 ...}} --folderoutput {{path/to/directory}}`

- Search for a specific username on social networks using the Tor network:

`sherlock --tor {{username}}`

- Make requests over Tor with a new Tor circuit after each request:

`sherlock --unique-tor {{username}}`

- Search for a specific username on social networks using a proxy:

`sherlock {{username}} --proxy {{proxy_url}}`

- Search for a specific username on social networks and open results in the default web browser:

`sherlock {{username}} --browse`

- Display help:

`sherlock --help`
