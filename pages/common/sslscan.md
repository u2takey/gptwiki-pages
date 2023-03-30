# sslscan 
## chatgpt 
sslscan is a command-line tool used to test SSL/TLS enabled services to determine the level of security offered by them. It is designed to identify misconfigurations, weak ciphers, and vulnerabilities in SSL/TLS based services. 

The syntax of the command is: 

sslscan [options] [hostname][:port] 

Here, hostname is the name of the server, and port is the port number on which the service is running. If no port is specified, the default port for the particular protocol will be used (443 for HTTPS, 995 for POP3S, 993 for IMAPS, and so on). 

Some of the options that can be used with sslscan include -h to display help, -V to display version information, -b to perform basic checks only, -r to report unsupported ciphers, and so on. 

When run, sslscan connects to the specified server and initiates the SSL/TLS handshake to determine which protocols and cipher suites are supported. It then tests each supported cipher suite for vulnerabilities and reports the results. 

The output from sslscan includes a summary of the scan results along with details such as the cipher suite used, encryption strength, and SSL/TLS version. It also identifies any weaknesses or vulnerabilities found, such as the use of weak ciphers or outdated SSL/TLS protocols. 

Overall, sslscan is a useful tool for system administrators and security professionals to assess the security of their SSL/TLS enabled services, and to identify any potential vulnerabilities or weaknesses that can be exploited by attackers. 

## tldr 
 
> Check SSL/TLS protocols and ciphers supported by a server.
> More information: <https://github.com/rbsec/sslscan>.

- Test a server on port 443:

`sslscan {{example.com}}`

- Test a specified port:

`sslscan {{example.com}}:{{465}}`

- Show certificate information:

`testssl --show-certificate {{example.com}}`
