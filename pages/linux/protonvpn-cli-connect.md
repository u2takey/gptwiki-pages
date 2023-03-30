# protonvpn-cli connect 
## chatgpt 
The `protonvpn-cli connect` command initiates a connection to the ProtonVPN service using the ProtonVPN command-line interface (CLI).

Here's a breakdown of the command:

- `protonvpn-cli`: This is the name of the ProtonVPN CLI executable file.
- `connect`: This is the command that tells the ProtonVPN CLI to initiate a connection to the ProtonVPN service.

When executed, this command will connect your device to the ProtonVPN network, allowing you to browse the internet securely and anonymously through a VPN tunnel. The specific location that you are connected to will depend on your account settings, as well as any flags or arguments that you specify when running the command. 

## tldr 
 
> Official client to connect to ProtonVPN from the command-line.
> More information: <https://protonvpn.com/support/linux-vpn-setup/>.

- Connect to ProtonVPN interactively:

`protonvpn-cli connect`

- Connect to ProtonVPN using the fastest server available:

`protonvpn-cli connect --fastest`

- Connect to ProtonVPN using a specific server with a specific protocol:

`protonvpn-cli connect {{server_name}} --protocol {{udp|tcp}}`

- Connect to ProtonVPN using a random server with a specific protocol:

`protonvpn-cli connect --random --protocol {{udp|tcp}}`

- Connect to ProtonVPN using the fastest Tor-supporting server:

`protonvpn-cli connect --tor`

- Display help:

`protonvpn-cli connect --help`
