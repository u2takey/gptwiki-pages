# sshfs 
## chatgpt 
The SSHFS command is used to mount a remote file system on a local machine securely over a Secure Shell (SSH) connection. This allows users to access files and directories on remote servers as if they were local files and directories, making it easy to transfer files between remote servers and local machines.

The command followed by sshfs is as follows:

```
sshfs user@server:/remote/dir /local/mount/point
```

In the above command:

- `user` is the username of the user on the remote server.
- `server` is the IP address or domain name of the remote server.
- `/remote/dir` is the path of the remote directory that you want to mount.
- `/local/mount/point` is the path of the local directory where you want to mount the remote file system.

After executing the command, the user will be prompted for the password of their account on the remote server to authenticate the SSH connection. Once authenticated, the remote directory becomes accessible via the local mount point just like any other local directory.

To unmount the SSH file system, use the following command:

```
umount /local/mount/point
```

The SSHFS command is a useful tool for remote file system management and works seamlessly with popular file managers such as Nautilus, Thunar, and PCManFM. 

## tldr 
 
> Filesystem client based on SSH.
> More information: <https://github.com/libfuse/sshfs>.

- Mount remote directory:

`sshfs {{username}}@{{remote_host}}:{{remote_directory}} {{mountpoint}}`

- Unmount remote directory:

`umount {{mountpoint}}`

- Mount remote directory from server with specific port:

`sshfs {{username}}@{{remote_host}}:{{remote_directory}} -p {{2222}}`

- Use compression:

`sshfs {{username}}@{{remote_host}}:{{remote_directory}} -C`

- Follow symbolic links:

`sshfs -o follow_symlinks {{username}}@{{remote_host}}:{{remote_directory}} {{mountpoint}}`
