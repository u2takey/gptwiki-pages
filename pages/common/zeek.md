# zeek 
## chatgpt 
Zeek is an open-source network security monitoring tool used to analyze network traffic and detect security issues. When you run the command "zeek" on a terminal or command prompt, it starts the Zeek script interpreter and initiates network monitoring. 

The Zeek script interpreter reads configuration files and scripts, which define the types of network events to log and how to analyze them. It uses a modular design with plugins that provide additional functionality, such as protocol analyzers and file extractors.

Once Zeek is running, it captures network traffic and either logs it to files or sends it to a real-time dashboard for immediate analysis. Zeek can detect a wide range of security threats, including malware infections, network traffic misuse, and attempts to exploit vulnerabilities in systems.

Overall, the zeek command is the main way to run and interact with the Zeek network security monitoring tool, making it an essential tool for network administrators and cybersecurity professionals. 

## tldr 
 
> Passive network traffic analyzer.
> Any output and log files will be saved to the current working directory.
> More information: <https://docs.zeek.org/en/lts/quickstart.html#zeek-as-a-command-line-utility>.

- Analyze live traffic from a network interface:

`sudo zeek --iface {{interface}}`

- Analyze live traffic from a network interface and load custom scripts:

`sudo zeek --iface {{interface}} {{script1}} {{script2}}`

- Analyze live traffic from a network interface, without loading any scripts:

`sudo zeek --bare-mode --iface {{interface}}`

- Analyze live traffic from a network interface, applying a `tcpdump` filter:

`sudo zeek --filter {{path/to/filter}} --iface {{interface}}`

- Analyze live traffic from a network interface using a watchdog timer:

`sudo zeek --watchdog --iface {{interface}}`

- Analyze traffic from a `pcap` file:

`zeek --readfile {{path/to/file.trace}}`
