# openfortivpn 
## chatgpt 
openfortivpn is a command-line VPN client application that provides secure, reliable, and feature-rich VPN connectivity to remote networks. It is designed specifically for FortiGate devices, a brand of network security devices manufactured by Fortinet, Inc. 

When you run the 'openfortivpn' command, it will launch the VPN client and allow you to connect to a remote network using FortiGate devices. The application will prompt you to enter the necessary VPN credentials, such as the username and password, to establish the connection.

Some of the features of openfortivpn include support for multiple authentication methods, automatic routing of traffic through the VPN connection, and the ability to reconnect automatically if the connection gets disconnected. It is also easy to use, with a simple and intuitive command-line interface that lets you control various aspects of the VPN connection.

Overall, openfortivpn is a powerful and flexible VPN client that provides secure and reliable VPN connectivity, making it an excellent choice for individuals and organizations looking to connect to remote networks using FortiGate devices. 

## tldr 
 
> A VPN client, for Fortinet's proprietary PPP+SSL VPN solution.
> More information: <https://github.com/adrienverge/openfortivpn>.

- Connect to a VPN with a username and password:

`openfortivpn --username={{username}} --password={{password}}`

- Connect to a VPN using a specific configuration file (defaults to `/etc/openfortivpn/config`):

`sudo openfortivpn --config={{path/to/config}}`

- Connect to a VPN by specifying the host and port:

`openfortivpn {{host}}:{{port}}`

- Trust a given gateway by passing in its certificate's sha256 sum:

`openfortivpn --trusted-cert={{sha256_sum}}`
