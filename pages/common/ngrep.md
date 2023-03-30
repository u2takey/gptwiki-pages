# ngrep 
## chatgpt 
ngrep is a command-line tool used to capture and display network traffic between your machine and other machines on the network. This tool is similar to tcpdump, but it offers additional features like filtering options, regular expression matching, etc. 

The basic syntax of the command is:

```
ngrep [options] filter expression
```

Here's how to interpret each part of the command:

- ngrep: This is the command itself.
- options: ngrep has several options that can be used to customize the output and filters applied. For example, -q option will quiet the output and -d option allows specifying the network interface to monitor.
- filter: This refers to the network traffic (based on the communication protocol) you want to capture. For instance, if you want to intercept network traffic using HTTP, the filter option would be 'tcp port 80'.
- expression: This specifies what to search for within the network traffic. It is used in combination with a filter to locate specific data. The expression is usually a regular expression pattern that specifies what type of data you are looking for.

Once you have configured the options, filters, and expressions, ngrep will start capturing the specified network traffic and display it in real-time on the command-line interface. The output contains details like source and destination IP addresses, source and destination ports, packet payloads, and more. By analyzing this output, you can gain valuable insights into network activity, troubleshoot connectivity issues, etc. 

## tldr 
 
> Filter network traffic packets using regular expressions.
> More information: <https://github.com/jpr5/ngrep>.

- Capture traffic of all interfaces:

`ngrep -d any`

- Capture traffic of a specific interface:

`ngrep -d {{eth0}}`

- Capture traffic crossing port 22 of interface eth0:

`ngrep -d {{eth0}} port {{22}}`

- Capture traffic from or to a host:

`ngrep host {{www.example.com}}`

- Filter keyword 'User-Agent:' of interface eth0:

`ngrep -d {{eth0}} '{{User-Agent:}}'`
