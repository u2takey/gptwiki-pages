# tailscale up 
## chatgpt 
"Tailscale up" is a command used to start the Tailscale networking service. Tailscale is a virtual private network (VPN) product that offers secure and private network connections on the internet. 

When the "tailscale up" command is executed, the Tailscale service will be started, and a secure virtual network will be created between the connected devices. This enables secure communication and data transfer between devices, regardless of their physical location or network configuration.

To use the "tailscale up" command, you will need to install Tailscale on your device or server. Once installed, you can run the command from the command-line interface and follow the on-screen prompts to connect to the Tailscale network. 

Overall, the "tailscale up" command is a quick and easy way to initiate the Tailscale VPN service and connect to a secure and private network. 

## tldr 
 
> Connects the client to the Tailscale network.
> In version 1.8 and above, command line arguments are stored and reused until they're overwritten or `--reset` is called.
> More information: <https://tailscale.com/kb/admin/>.

- Connect to Tailscale:

`sudo tailscale up`

- Connect and offer the current machine to be an exit node for internet traffic:

`sudo tailscale up --advertise-exit-node`

- Connect using a specific node for internet traffic:

`sudo tailscale up --exit-node={{exit_node_ip}}`

- Connect and block incoming connections to the current node:

`sudo tailscale up --shields-up`

- Connect and don't accept DNS configuration from the admin panel (defaults to `true`):

`sudo tailscale up --accept-dns={{false}}`

- Connect and configure Tailscale as a subnet router:

`sudo tailscale up --advertise-routes={{10.0.0.0/24}},{{10.0.1.0/24}}`

- Connect and accept subnet routes from Tailscale:

`sudo tailscale up --accept-routes`

- Reset unspecified settings to their default values and connect:

`sudo tailscale up --reset`
