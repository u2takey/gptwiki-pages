# sftp 
## chatgpt 
The sftp command is used to securely transfer files over a network using the Secure File Transfer Protocol (SFTP). It is a command-line utility that allows users to transfer files between local and remote systems securely. 

The syntax of the sftp command is as follows: 

```
sftp [OPTIONS] [USER@]HOST
```

Here, `[OPTIONS]` are any additional command-line options needed for the specified operation, `[USER@]` specifies the username for the remote host, and `HOST` is the name or IP address of the remote system.

When you run the sftp command, it establishes a secure shell (SSH) connection to the remote host and provides a terminal-like interface where you can perform various file transfer operations. The sftp prompt looks similar to a shell prompt, but with an `sftp>` prefix. 

Some common uses of the sftp command include uploading and downloading files, creating and deleting directories, and listing remote directories' contents. 

Below are some examples of using the sftp command:

1. To connect to a remote host and start an sftp session:

```
sftp username@remote-host
```

2. To upload a local file to the remote host:

```
put localfile.txt remotefile.txt
```

3. To download a remote file to the local system:

```
get remotefile.txt localfile.txt
```

4. To create a new directory on the remote host:

```
mkdir newdirectory
```

5. To delete a remote file:

```
rm remotefile.txt
```

Overall, the sftp command is an essential utility for securely transferring files between local and remote systems. 

## tldr 
 
> Secure File Transfer Program.
> Interactive program to copy files between hosts over SSH.
> For non-interactive file transfers, see `scp` or `rsync`.
> More information: <https://manned.org/sftp>.

- Connect to a remote server and enter an interactive command mode:

`sftp {{remote_user}}@{{remote_host}}`

- Connect using an alternate port:

`sftp -P {{remote_port}} {{remote_user}}@{{remote_host}}`

- Connect using a predefined host (in `~/.ssh/config`):

`sftp {{host}}`

- Transfer remote file to the local system:

`get {{/path/remote_file}}`

- Transfer local file to the remote system:

`put {{/path/local_file}}`

- Transfer remote directory to the local system recursively (works with `put` too):

`get -R {{/path/remote_directory}}`

- Get list of files on local machine:

`lls`

- Get list of files on remote machine:

`ls`
