# chronyc 
## chatgpt 
Chronyc is a command-line tool for controlling the NTP daemon (Network Time Protocol) called Chronyd, which is responsible for synchronizing the system clock of a computer with reliable time sources on the internet. Chronyc is used to perform various tasks related to time synchronization, such as querying status and statistics, configuring options, troubleshooting, and adjusting the clock.

The syntax of the chronyc command is as follows:

chronyc [options] [command] [arguments]

Options: 
- -h, --help: shows a help message.
- -n, --nocolor: disables color output.
- -r, --remote=ADDR: specifies the NTP server address or hostname to use.
- -s, --source=ADDRESS: specifies the IP address or network interface to use for communication.
- -f, --file=FILENAME: specifies an alternate configuration file.

Commands:
- tracking: shows the current tracking and clock statistics.
- sources: displays the list of time sources used by chronyd.
- sourcestats: shows the statistics of each time source.
- sourceshift: shows the offset between each time source and the system clock.
- sourcestats2: shows detailed statistics of each time source.
- makestep: sets the system clock to the NTP server time immediately.
- online: turns the NTP synchronization on.
- offline: turns the NTP synchronization off.
- burst: sends a burst of NTP requests to the server and displays the response.
- quit: exits the chronyc shell.

Overall, the chronyc command is a powerful utility that enables users to manage the time synchronization of their system clocks with precision and accuracy. It is particularly useful in environments that require high levels of time synchronization, such as financial trading platforms, scientific research, and industrial control systems. 

## tldr 
 
> Query the Chrony NTP daemon.
> More information: <https://chrony.tuxfamily.org/doc/4.0/chronyc.html>.

- Start chronyc in interactive mode:

`chronyc`

- Display tracking stats for the Chrony daemon:

`chronyc tracking`

- Print the time sources that Chrony is currently using:

`chronyc sources`

- Display stats for sources currently used by chrony daemon as a time source:

`chronyc sourcestats`

- Step the system clock immediately, bypassing any slewing:

`chronyc makestep`

- Display verbose information about each NTP source:

`chronyc ntpdata`
