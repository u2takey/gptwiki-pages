# ntpdate 
## chatgpt 
"ntpdate" is a simple command line utility that is used to set the date and time on a computer system by synchronizing it with an NTP (Network Time Protocol) server. 

The syntax for the ntpdate command is as follows:

```ntpdate [options] [server]```

Options:
- -u : Use an unprivileged network port instead of the privileged port (123)
- -b : Use a non-step mode for synchronization with the time server
- -d : Debugging output level
- -s : Set the time immediately without slewing

Server:
- The NTP server is the source of time synchronization. You can enter the IP address or hostname of an NTP server in this field.

When running the ntpdate command, the computer sends a request to the specified NTP server to obtain the current time information. The server then responds with the precise date and time information, which the computer uses to update its clock.

Once the clock of the computer system is synchronized with the NTP server, it will maintain the correct date and time, and adjust it automatically when the server updates its own time information. This ensures that the time on the computer is always accurate and consistent with other devices on the network. 

## tldr 
 
> Synchronize and set the date and time via NTP.
> More information: <http://support.ntp.org/documentation>.

- Synchronize and set date and time:

`sudo ntpdate {{host}}`

- Query the host without setting the time:

`ntpdate -q {{host}}`

- Use an unprivileged port in case a firewall is blocking privileged ports:

`sudo ntpdate -u {{host}}`

- Force time to be stepped using `settimeofday` instead of `slewed`:

`sudo ntpdate -b {{host}}`
