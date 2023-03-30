# apt-key 
## chatgpt 
apt-key is a command-line tool and a management tool that manipulates authentication keys used to authenticate packages with Apt: GPG keys for secure updates, importing and exporting of package signing keys, and individual keys for repositories. 

In Ubuntu and Debian-based systems, Apt package manager uses GPG (GNU Privacy Guard) keys to authenticate packages before they are installed on the system. These keys are used to ensure that the packages are verified and safe to install. 

apt-key is used to manage these keys by importing, exporting, and deleting them. It also allows you to manage the trusted repositories so that you can download safe and trusted packages. 

Below are some common uses of the apt-key command:

- apt-key add: This command allows you to add a new key to the list of trusted keys for Apt. You can specify either a GPG key file or a URL that links to a key file.

- apt-key export: This command allows you to export a GPG key that you have added to Apt, into a file on disk.

- apt-key export-all: This command exports all the trusted keys managed by Apt into a file on disk.

- apt-key list: This command lists all the keys that have been added or imported to Apt.

- apt-key del: This command allows you to delete a key from the list of trusted keys for Apt. 

Overall, apt-key is a useful tool that helps ensure the integrity and security of packages being installed through the Apt package manager. 

## tldr 
 
> Key management utility for the APT Package Manager on Debian and Ubuntu.
> Note: `apt-key` is now deprecated (except for the use of `apt-key del` in maintainer scripts).
> More information: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

- List trusted keys:

`apt-key list`

- Add a key to the trusted keystore:

`apt-key add {{public_key_file.asc}}`

- Delete a key from the trusted keystore:

`apt-key del {{key_id}}`

- Add a remote key to the trusted keystore:

`wget -qO - {{https://host.tld/filename.key}} | apt-key add -`

- Add a key from keyserver with only key id:

`apt-key adv --keyserver {{pgp.mit.edu}} --recv {{KEYID}}`
