# hping3 
## chatgpt 
hping3 is a command-line tool used for network exploration, security auditing, and testing of firewall and intrusion detection systems. It is a versatile and powerful tool that offers a lot of features for network packet analysis and manipulation.

Here are some of the main features and common usages of hping3:

- Ping/Traceroute: hping3 can be used to send ICMP, UDP, or TCP packets to a target host or network and measure the response time or route. This is useful for testing network connectivity, detecting firewalls or NATs, and diagnosing network issues.

- Port scanning: hping3 can perform various types of port scans, including TCP connect(), SYN stealth(), FIN stealth(), Xmas stealth(), and NULL stealth(). These techniques can help identify open ports and services running on a host or network, as well as stealthily avoid detection by intrusion prevention systems.

- Packet crafting: hping3 allows you to create or modify custom packets and send them to a target host or network. This is useful for testing application or network vulnerabilities, simulating attacks, and bypassing filters or authentication mechanisms.

- DoS/DDoS: hping3 can be used as a tool for launching Denial of Service (DoS) or Distributed Denial of Service (DDoS) attacks by flooding a target host or network with a high volume of network traffic. However, such usage is illegal and unethical, and should not be attempted without permission or proper authorization.

Overall, hping3 is a powerful and flexible tool for network testing and security analysis, but it requires a good understanding of networking principles and protocols to use effectively and responsibly. 

## tldr 
 
> Advanced ping utility which supports protocols such TCP, UDP, and raw IP.
> Best run with elevated privileges.
> More information: <https://github.com/antirez/hping>.

- Ping a destination with 4 ICMP ping requests:

`hping3 --icmp --count {{4}} {{ip_or_hostname}}`

- Scan TCP port 80, scanning from the specific local source port 5090:

`hping3 --verbose --syn --destport {{80}} --baseport {{5090}} {{ip_or_hostname}}`

- Traceroute using a TCP scan to a specific destination port:

`hping3 --traceroute --verbose --syn --destport {{80}} {{ip_or_hostname}}`

- Perform a TCP ACK scan to check if a given host is alive:

`hping3 --count {{2}} --verbose --destport {{80}} -A {{ip_or_hostname}}`
