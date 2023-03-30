# nmcli agent 
## chatgpt 
The "nmcli agent" command is used to control the NetworkManager. 

The "nmcli" is a command-line tool for controlling and displaying the status of NetworkManager. It stands for "Network Manager Command-Line Interface".

The "agent" argument is used to interact with the NetworkManager agent. The agent is a component of NetworkManager that runs as a daemon and provides advanced network configuration and manage network devices. 

Using "nmcli agent", you can manage and control the behavior of the NetworkManager agent. It supports several subcommands, such as "status", "start", "stop", and "restart". 

For example, "nmcli agent status" will display the current status of the NetworkManager agent, while "nmcli agent start" will start the agent if it's not already running. Similarly, "nmcli agent stop" will stop the agent, and "nmcli agent restart" will restart it. 

Overall, the "nmcli agent" command is useful for managing the NetworkManager agent, which is essential for network configuration on many Linux systems. 

## tldr 
 
> Run nmcli as a NetworkManager secret agent or polkit agent.
> This subcommand can also be called with `nmcli a`.
> More information: <https://networkmanager.dev/docs/api/latest/nmcli.html>.

- Register nmcli as a secret agent and listen for secret requests:

`nmcli agent secret`

- Register nmcli as a polkit agent and listen for authorization requests:

`nmcli agent polkit`

- Register nmcli as a secret agent and a polkit agent:

`nmcli agent all`
