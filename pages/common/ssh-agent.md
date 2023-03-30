# ssh-agent 
## chatgpt 
The `ssh-agent` command is used to start an SSH agent, which is a program that manages private SSH keys.

When an SSH agent is running, it stores your private keys in memory and can be used to authenticate SSH connections without requiring you to enter your password each time. The agent will prompt you to enter your passphrase once, and then remember it for the rest of the session.

The `ssh-agent` command is usually run automatically when you start an SSH session, but you can also run it manually to start a standalone agent. Once the agent is running, you can add your keys to it using the `ssh-add` command, which will prompt you for your passphrase.

Overall, the `ssh-agent` command is a useful tool for managing your SSH keys and can help streamline your SSH workflow. 

## tldr 
 
> Spawn an SSH Agent process.
> An SSH Agent holds SSH keys decrypted in memory until removed or the process is killed.
> See also `ssh-add`, which can add and manage keys held by an SSH Agent.
> More information: <https://man.openbsd.org/ssh-agent>.

- Start an SSH Agent for the current shell:

`eval $(ssh-agent)`

- Kill the currently running agent:

`ssh-agent -k`
