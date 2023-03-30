# hping 
## chatgpt 
Hping is a command line tool used for network testing and troubleshooting. It is a packet generator and analyzer that allows its users to send and analyze custom packets to determine network performance, security and reliability. The main features of Hping include:

1. Fingerprinting: Hping is used to identify the operating system or application running on a remote host by sending specific TCP or ICMP packets, and analyzing the responses.

2. Ping: Hping can be used to test network connectivity and packet loss by sending ICMP echo request packets to a remote host.

3. Traceroute: With this feature, Hping can trace the routing path taken by packets to reach their destination.

4. Port scanning: Hping can send TCP or UDP packets to a range of ports on a remote host to determine which ports are open or closed.

5. DoS attacks: Using Hping, users can simulate different types of DoS (Denial of Service) attacks, such as SYN flood, UDP flood, and ICMP flood.

The command-line syntax for Hping includes various options and flags, which allow users to customize their packet generation and analysis. Some common options include:

- -c: specify the number of packets to be sent
- -k: keep sending packets until interrupted
- -S: set the TCP SYN flag
- -R: set the TCP RST flag
- -P: set the UDP protocol
- -I: set the ICMP protocol
- -t: specify the TTL (Time to Live) value for packets

Overall, Hping is a powerful and versatile network testing tool that can be used for a wide range of purposes, from packet generation and analysis to diagnosing network problems and security testing. 

## tldr 
 
> Command-line oriented TCP/IP packet assembler and analyzer.
> Inspired by the `ping` command.
> More information: <http://www.hping.org>.

- Ping localhost over TCP:

`hping3 {{localhost}}`

- Ping an IP address over TCP on a specific port:

`hping3 -p {{80}} -S {{192.168.1.1}}`

- Ping an IP address over UDP on port 80:

`hping3 --udp -p {{80}} -S {{192.168.1.1}}`

- Scan a set of TCP ports on a specific IP address:

`hping3 --scan {{80,3000,9000}} -S {{192.168.1.1}}`

- Perform a charge test on port 80:

`hping3 --flood -p {{80}} -S {{192.168.1.1}}`
