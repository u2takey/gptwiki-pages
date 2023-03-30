# pssh 
## chatgpt 
The command "pssh" stands for "parallel-ssh". This command is a tool that enables users to run commands across multiple remote servers simultaneously, in parallel. 

With pssh, users can perform various tasks, including running commands on multiple servers, copying files to multiple servers, gathering output from multiple servers, and more.

The basic syntax of pssh command is:

pssh [options] command 

Here are some of the important options frequently used with the pssh command:

- -h: Specifies the file containing a list of hosts to run the command on.
- -l: Specifies the username to use for logging into the remote host.
- -P: Specifies the maximum number of concurrent connections that can be established at a time.
- -i: Specifies the identity file for public key authentication.

Overall, pssh is a powerful tool for managing multiple servers at once, and it can save a significant amount of time and effort for system administrators and IT professionals. 

## tldr 
 
> Parallel SSH program.
> More information: <https://manned.org/pssh>.

- Run a command on two hosts, and print its output on each server inline:

`pssh -i -H "{{host1}} {{host2}}" {{hostname -i}}`

- Run a command and save the output to separate files:

`pssh -H {{host1}} -H {{host2}} -o {{path/to/output_dir}} {{hostname -i}}`

- Run a command on multiple hosts, specified in a new-line separated file:

`pssh -i -h {{path/to/hosts_file}} {{hostname -i}}`

- Run a command as root (this asks for the root password):

`pssh -i -h {{path/to/hosts_file}} -A -l {{root_username}} {{hostname -i}}`

- Run a command with extra SSH arguments:

`pssh -i -h {{path/to/hosts_file}} -x "{{-O VisualHostKey=yes}}" {{hostname -i}}`

- Run a command limiting the number of parallel connections to 10:

`pssh -i -h {{path/to/hosts_file}} -p {{10}} '{{cd dir; ./script.sh; exit}}'`
