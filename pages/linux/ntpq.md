# ntpq 
## chatgpt 
The `ntpq` command is a utility program used to query and troubleshoot the Network Time Protocol (NTP) daemon running on a Unix/Linux based computer system. It is commonly used by system administrators to verify that the computer's time is synchronized with a reliable time source.

When you run the `ntpq` command in the terminal, you will be presented with an interactive shell that allows you to query a local or remote NTP server. Here are some examples of useful commands you can execute in the `ntpq` shell:

1. `ntpq -p`: This command displays a list of the NTP servers or peers that your system is currently synchronized to. It shows the IP address or host name of each server, the Stratum level, and the time offset from your local system clock.

2. `ntpq -c peers`: This command provides a summary of the peers known to the NTP daemon. It shows information such as the IP address, reference ID, and leap status for each peer.

3. `ntpq -c associations`: Similar to the previous command, this command provides an overview of the associations between your system and the NTP servers it is communicating with.

4. `ntpq -c rv`: This command displays information about the last seen reachability of the remote NTP peers.

5. `ntpq -c sysinfo`: This command shows detailed information about the local clock and its current configuration.

6. `ntpq -c clockvar`: This command displays estimated accuracy and measurement uncertainty of the local clock.

7. `ntpq -c iostats`: This command shows statistics about the INPUT/OUTPUT operations on the system.

Overall, the `ntpq` command provides a useful set of tools for system administrators to troubleshoot and maintain accurate time synchronization between their computer systems and external NTP servers. 

## tldr 
 
> Query the Network Time Protocol (NTP) daemon.
> More information: <https://www.eecis.udel.edu/~mills/ntp/html/ntpq.html>.

- Start `ntpq` in interactive mode:

`ntpq --interactive`

- Print a list of NTP peers:

`ntpq --peers`

- Print a list of NTP peers without resolving hostnames from IP addresses:

`ntpq --numeric --peers`

- Use `ntpq` in debugging mode:

`ntpq --debug-level`

- Print NTP system variables values:

`ntpq --command={{rv}}`
