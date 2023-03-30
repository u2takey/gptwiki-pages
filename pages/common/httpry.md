# httpry 
## chatgpt 
The httpry command is a network traffic monitoring tool that captures and displays HTTP traffic in real-time. The command works by monitoring HTTP traffic over a network interface and analyzing the traffic to identify key details about each HTTP request and response.

When you run the httpry command, it captures all HTTP traffic on the specified network interface and displays a detailed summary of each request and response. This summary includes details such as the source and destination IP addresses, the HTTP method used, the requested URL, and the HTTP status code.

The httpry command also provides several options for filtering and sorting the captured traffic to make it easier to analyze. For example, you can filter out traffic from specific IP addresses or only display requests and responses for certain HTTP methods.

Overall, the httpry command is a useful tool for developers and network engineers who need to monitor and troubleshoot HTTP traffic on a network. It provides a detailed and real-time view of all HTTP traffic, making it easier to identify and resolve issues quickly. 

## tldr 
 
> A lightweight packet sniffer for displaying and logging HTTP traffic.
> It can be run in real-time displaying the traffic as it is parsed, or as a daemon process that logs to an output file.
> More information: <http://dumpsterventures.com/jason/httpry/>.

- Save output to a file:

`httpry -o {{path/to/file.log}}`

- Listen on a specific interface and save output to a binary pcap format file:

`httpry {{eth0}} -b {{path/to/file.pcap}}`

- Filter output by a comma-separated list of HTTP verbs:

`httpry -m {{get|post|put|head|options|delete|trace|connect|patch}}`

- Read from an input capture file and filter by IP:

`httpry -r {{path/to/file.log}} '{{host 192.168.5.25}}'`

- Run as daemon process:

`httpry -d -o {{path/to/file.log}}`
