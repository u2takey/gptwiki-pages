# pppd 
## chatgpt 
The pppd command is used to establish a Point-to-Point Protocol (PPP) connection between two computers over a serial interface, such as connecting to the internet over a phone line or creating a remote access connection to a network.

The basic syntax for the pppd command is:

```
pppd [options] <serial_device> <speed> [modem_option]
```

where `serial_device` is the name of the serial port that the modem is connected to (e.g. `/dev/ttyS0`), `speed` is the speed of the serial port (e.g. 9600), and `modem_option` is any additional command-line options that the modem requires.

Some common options for the pppd command are:

- `-detach`: Run in the background as a daemon.
- `-defaultroute`: Add a default route to the routing table to send all outgoing traffic through the PPP connection.
- `-auth`: Require authentication using the PAP or CHAP protocol.
- `-noauth`: Don't require authentication.
- `-mru`: Set the Maximum Receive Unit (MRU) size for the PPP connection.
- `-mtu`: Set the Maximum Transmission Unit (MTU) size for the PPP connection.
- `-debug`: Print debugging messages to the console.

Once the PPP connection is established, the pppd command will manage the connection and negotiate the PPP protocol with the remote computer. The connection can be terminated by sending a signal to the pppd process (e.g. `killall pppd`). 

## tldr 
 
> Establish Point-to-Point connection to another computer.
> It should not be invoked manually.
> More information: <https://ppp.samba.org/pppd.html>.

- Start the daemon:

`pppd`
