# sshd 
## chatgpt 
sshd is a system daemon that allows secure remote access to a computer running Linux or other Unix-like operating systems. 

When a user wants to remotely access a server using SSH, the sshd daemon receives the incoming SSH connection request and grants access only if the username and password are correct. The sshd daemon is responsible for managing the secure shell (SSH) protocol, which ensures that information exchanged between the server and the client is encrypted and secure.

The sshd command is used to start, stop, or restart the sshd daemon. When the sshd daemon is started on a system, it listens for incoming SSH connections on the default port 22. The sshd command configures and controls the behaviour of the SSH server.

Syntax: 

sshd [-DdpqTCcfxeghkKnN] [-b bits] [-E log_file] [-f 
config_file] [-g login_grace_time] [-h host_key_file] 
[-o option] [-p port] [-u len] [user_group1 ...]

Here are some of the commonly used options of the sshd command:
- -D: Do not detach and run in the foreground.
- -p: Specifies the port to listen on for incoming SSH connections.
- -f: Specifies the configuration file for the sshd daemon.
- -s: Specifies the general configuration settings for the system's sshd daemon. 

In general, the sshd command is needed to run the secure shell server, which is necessary for secure remote access to a system. 

## tldr 
 
> Secure Shell Daemon - allows remote machines to securely log in to the current machine.
> Remote machines can execute commands as it is executed at this machine.
> More information: <https://man.openbsd.org/sshd>.

- Start daemon in the background:

`sshd`

- Run sshd in the foreground:

`sshd -D`

- Run with verbose output (for debugging):

`sshd -D -d`

- Run on a specific port:

`sshd -p {{port}}`
