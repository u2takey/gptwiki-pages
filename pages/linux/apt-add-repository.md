# apt-add-repository 
## chatgpt 
The `apt-add-repository` command is used in Debian and Ubuntu-based Linux distributions to add a third-party repository to the local package manager's list of sources. 

Here's a breakdown of the various components of the command and what they do:

- `apt-add-repository`: This is the name of the command that we're executing.
- The options that can be passed to this command are:
  - `-y`: Skip the confirmation prompt when adding the repository
  - `-u`: Update the local package list after adding the repository
  - `-n`: Skip adding a new Debian package signing key
  - `-r`: Remove an existing repository from the list
  - `-s`: Add a source repository, which includes the source code for the packages in addition to the compiled packages
- Repository details: After the options have been specified, we need to provide the details of the repository we want to add. This typically includes a URL for the repository and a code name for the distribution (e.g. `focal` for Ubuntu 20.04).
- GPG key: If the repository has a GPG key that needs to be imported to verify package signatures, we can add it using the `wget` and `apt-key` commands.

Here's an example command that adds the MongoDB public GPG key and repository to an Ubuntu system:

```
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10
sudo apt-add-repository 'deb [arch=amd64] https://repo.mongodb.org/apt/ubuntu bionic/mongodb-org/4.4 multiverse'
sudo apt update
```

- The first line imports the MongoDB public GPG key so that the package manager can verify the authenticity of packages from this repository.
- The second line adds the repository using the `-y` option to automatically confirm the prompt.
- The third line updates the local package list to include packages from the newly added repository. 

## tldr 
 
> Manages apt repository definitions.
> More information: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

- Add a new apt repository:

`apt-add-repository {{repository_spec}}`

- Remove an apt repository:

`apt-add-repository --remove {{repository_spec}}`

- Update the package cache after adding a repository:

`apt-add-repository --update {{repository_spec}}`

- Enable source packages:

`apt-add-repository --enable-source {{repository_spec}}`
