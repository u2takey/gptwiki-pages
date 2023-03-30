# openvpn 
## chatgpt 
OpenVPN is an open-source Virtual Private Network (VPN) software. It allows you to create secure connections between computers over the internet. The command "openvpn" is used to launch and control the OpenVPN service. 

When you run the "openvpn" command, it starts the OpenVPN client and connects to the configured VPN server. The configuration file for the VPN connection is passed as an argument to the command. 

Here are some common options that can be used with the "openvpn" command:

- --config filename - Specifies the configuration file for the VPN connection.
- --daemon - Runs OpenVPN in the background.
- --log file - Writes debug messages to a log file.
- --auth user/pass - Specifies the username and password for authentication.
- --verb level - Specifies the verbosity level of the log output.

Once the OpenVPN client is connected to the VPN server, it creates a secure tunnel for all data to pass through. This tunnel is encrypted using SSL/TLS protocols, which ensures that all data transmitted between the client and server is secure and cannot be intercepted or read by unauthorized parties. 

In summary, the "openvpn" command is used to launch and control the OpenVPN client, enabling secure connections between computers over the internet. 

## tldr 
 
> OpenVPN client and daemon binary.
> More information: <https://openvpn.net/>.

- Connect to server using a config file:

`sudo openvpn {{path/to/client.conf}}`

- Try to set up an insecure peer-to-peer tunnel on bob.example.com host:

`sudo openvpn --remote {{alice.example.com}} --dev {{tun1}} --ifconfig {{10.4.0.1}} {{10.4.0.2}}`

- Connect to the awaiting bob.example.com host without encryption:

`sudo openvpn --remote {{bob.example.com}} --dev {{tun1}} --ifconfig {{10.4.0.2}} {{10.4.0.1}}`

- Create a cryptographic key and save it to file:

`openvpn --genkey secret {{path/to/key}}`

- Try to set up a peer-to-peer tunnel on bob.example.com host with a static key:

`sudo openvpn --remote {{alice.example.com}} --dev {{tun1}} --ifconfig {{10.4.0.1}} {{10.4.0.2}} --secret {{path/to/key}}`

- Connect to the awaiting bob.example.com host with the same static key as on bob.example.com:

`sudo openvpn --remote {{bob.example.com}} --dev {{tun1}} --ifconfig {{10.4.0.2}} {{10.4.0.1}} --secret {{path/to/key}}`
