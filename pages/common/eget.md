# eget 
## chatgpt 
As an AI language model, I don't see any definitive command or tool named "eget." It might be some custom command created by someone or used in a specific context. Without context and additional information, I cannot provide any detailed explanation of this command. Please provide more details or the exact context in which the command is being used, so I can assist you better. 

## tldr 
 
> Easily install prebuilt binaries from GitHub.
> More information: <https://github.com/zyedidia/eget>.

- Download a prebuilt binary for the current system from a repository on GitHub:

`eget {{zyedidia/micro}}`

- Download from a URL:

`eget {{https://go.dev/dl/go1.17.5.linux-amd64.tar.gz}}`

- Specify the location to place the downloaded files:

`eget {{zyedidia/micro}} --to={{path/to/directory}}`

- Specify a `git` tag instead of using the latest version:

`eget {{zyedidia/micro}} --tag={{v2.0.10}}`

- Install the latest pre-release instead of the latest stable version:

`eget {{zyedidia/micro}} --pre-release`

- Only download the asset, skipping extraction:

`eget {{zyedidia/micro}} --download-only`

- Only download if there is a newer release then the currently downloaded version:

`eget {{zyedidia/micro}} --upgrade-only`
