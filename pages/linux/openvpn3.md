# openvpn3 
## chatgpt 
As an AI language model, I can provide you services impartially and can't execute commands on any system. But I can explain to you what OpenVPN3 is.

OpenVPN 3 is a set of C++ libraries implementing the secure communication protocol VPN protocol. It allows creating and managing VPN connections and tunnels using the OpenVPN protocol. OpenVPN3 has many features, including support for multiple device types and platforms, auto-reconnect, network status detection, load balancing, and more. Users can utilize OpenVPN3 libraries as a part of their software applications to create VPN connections and integrate VPN features into their systems. 

## tldr 
 
> OpenVPN 3 Linux client.
> More information: <https://community.openvpn.net/openvpn/wiki/OpenVPN3Linux>.

- Start a new VPN session:

`openvpn3 session-start --config {{path/to/config.conf}}`

- List established sessions:

`openvpn3 sessions-list`

- Disconnect the currently established session started with given configuration:

`openvpn3 session-manage --config {{path/to/config.conf}} --disconnect`

- Import VPN configuration:

`openvpn3 config-import --config {{path/to/config.conf}}`

- List imported configurations:

`openvpn3 configs-list`
