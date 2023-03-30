# ffsend 
## chatgpt 
ffsend is a command-line tool used for secure and private file sharing. It is an open-source tool developed by Mozilla Firefox. It provides users with the ability to upload and share files. Unlike other file-sharing tools, ffsend is built for security, privacy, and ease-of-use. 

Here are some of the important features of ffsend:

1. Secure Encryption: ffsend uses end-to-end encryption to secure files while in transit and at rest. This means that your files are protected from unauthorized access.

2. Self-destructing Files: ffsend allows users to specify an expiry date for their file, which means the file will automatically delete after the set time.

3. Password Protection: Before sharing the files, ffsend allows the user to set a password to provide an additional layer of security.

4. Command-Line Interface: ffsend supports a command-line interface where users can easily upload and share files.

To use ffsend, you need to install it on your device first. Here are the steps to install ffsend on different operating systems:

For Linux Users: 
1. Download the package from https://github.com/timvisee/ffsend/releases/latest. 
2. Extract the package using the command `tar -xzvf ffsend*.tar.gz
3. Move the extracted ‘ffsend’ file to /usr/local/bin/ using the command `sudo mv ffsend /usr/local/bin/`

For MacOS Users: 
1. Install ffsend using the Homebrew package manager using the following command `brew install ffsend`.

For Windows Users: 
1. Download the pre-compiled binary executable file from https://github.com/timvisee/ffsend/releases/latest.
2. Extract the downloaded file and place it in a location where you can easily access it.

Once you have installed ffsend, you can start using it via the command-line (terminal). Here are some examples of how to use the ffsend command:

To upload a file:

`ffsend upload /path/to/file`

To upload a file with a password:

`ffsend upload --password "supersecretpassword" /path/to/file`

To upload a file with an expiration date:

`ffsend upload --expiry 1w /path/to/file`

To download a file:

`ffsend download <FileLink>`

Overall, ffsend is a secure, easy-to-use, and open-source tool for file sharing. It provides strong encryption and privacy features, as well as the option to set passwords and expiry dates for shared files. 

## tldr 
 
> Easily and securely share files from command-line.
> More information: <https://gitlab.com/timvisee/ffsend>.

- Upload a file:

`ffsend upload {{path/to/file}}`

- Download a file:

`ffsend download {{url}}`

- Upload a file with password:

`ffsend upload {{path/to/file}} -p {{password}}`

- Download a file protected by password:

`ffsend download {{path/to/file}} -p {{password}}`

- Upload a file and allow 4 downloads:

`ffsend upload {{path/to/file}} -d {{4}}`
