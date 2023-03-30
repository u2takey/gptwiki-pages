# pyrit 
## chatgpt 
Pyrit is a command-line tool used for wireless network auditing purposes. It is used for cracking the WEP, WPA/WPA2 encrypted Wi-Fi passwords. The tool is based on Python and has numerous other features that can be used for efficient wireless network analysis. Pyrit uses cryptographic algorithms to crack the Wi-Fi passwords through brute force attacks.

Some of the uses of Pyrit are:

1. Wireless password cracking
2. Packet analysis
3. WPA-Half Handshake and Distributed attack
4. Hash generation
5. Attack signature generation

Pyrit comes with various command-line options that include the following:

- `benchmark`: this command is used to test the performance of the user's GPU and CPU to determine the best cracking speed.
- `analyze`: used to analyze the wireless network for attacks and vulnerabilities.
- `attack_db`: used to configure and manage the attack signature database in Pyrit.
- `batch`: used to batch the WPA handshakes for easy cracking.
- `caps_read`: used to read the packet capture file in Pyrit.
- `choose_gpu`: used to select the specific GPU that will be used for cracking.
- `eval`: used to evaluate Pyrit hashes.

Overall, Pyrit is a valuable tool for assessing the security of wireless networks and identifying vulnerabilities for remediation. Its wide range of features and flexible configuration options make it an essential tool for network security analysts and penetration testers. 

## tldr 
 
> WPA/WPA2 cracking tool using computational power.
> More information: <https://github.com/JPaulMora/Pyrit>.

- Display system cracking speed:

`pyrit benchmark`

- List available cores:

`pyrit list_cores`

- Set [e]SSID:

`pyrit -e "{{ESSID}}" create_essid`

- [r]ead and analyze a specific packet capture file:

`pyrit -r {{path/to/file.cap|path/to/file.pcap}} analyze`

- Read and [i]mport passwords to the current database:

`pyrit -i {{path/to/file}} {{import_unique_passwords|unique_passwords|import_passwords}}`

- Exp[o]rt passwords from database to a specific file:

`pyrit -o {{path/to/file}} export_passwords`

- Translate passwords with Pired Master Keys:

`pyrit batch`

- [r]ead the capture file and crack the password:

`pyrit -r {{path/to/file}} attack_db`
