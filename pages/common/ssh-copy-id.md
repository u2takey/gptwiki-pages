# ssh-copy-id 
## chatgpt 
The `ssh-copy-id` command is used to quickly and securely copy a user's public key to a remote server's authorized_keys file. This is especially useful for setting up SSH key-based authentication to a remote server, as it eliminates the need for a password when logging in.

The command works by simply appending the user's public key to the remote server's authorized_keys file, which allows the user to log in without needing to enter a password. This can save a lot of time and effort, especially if you regularly need to connect to the same remote server.

Here is a breakdown of the command:

- `ssh-copy-id`: This is the basic command, which tells the shell to run the `ssh-copy-id` utility.
- `-i`: This stands for "identity file", and specifies the location of the user's private key. If this option is not specified, the default location (~/.ssh/id_rsa) will be used.
- `-p`: This specifies the SSH port number to use. If this option is not specified, the default port (22) will be used.
- `<user>@<host>`: This specifies the remote server to copy the public key to. You'll need to replace `<user>` with your username on the remote server, and `<host>` with the remote server's hostname or IP address.

Here's an example of how you can use the command to copy your public key to a remote server:

```
ssh-copy-id -i ~/.ssh/mykey.pub -p 2222 alice@remote-server.example.com
```

This command will copy the contents of the `mykey.pub` file (which should be your public SSH key) to the `authorized_keys` file on the remote server at `remote-server.example.com`, using the SSH port number 2222. You'll need to enter your password once to authenticate with the remote server, but after that, you'll be able to log in without needing a password. 

## tldr 
 
> Install your public key in a remote machine's authorized_keys.
> More information: <https://manned.org/ssh-copy-id>.

- Copy your keys to the remote machine:

`ssh-copy-id {{username@remote_host}}`

- Copy the given public key to the remote:

`ssh-copy-id -i {{path/to/certificate}} {{username}}@{{remote_host}}`

- Copy the given public key to the remote with specific port:

`ssh-copy-id -i {{path/to/certificate}} -p {{port}} {{username}}@{{remote_host}}`
