# protonvpn-cli 
## chatgpt 
The command 'protonvpn-cli' refers to the ProtonVPN Command Line Interface (CLI) tool which is used for managing ProtonVPN connections and settings via the terminal/command prompt. The tool allows users to connect or disconnect to VPN servers, view their connection status, change server locations, and manage their VPN account.

The 'protonvpn-cli' command is followed by various arguments that perform specific functions, such as:

- 'protonvpn-cli login': prompts the user for their ProtonVPN account credentials and logs them in
- 'protonvpn-cli connect': connects the user to the VPN server with the recommended configuration
- 'protonvpn-cli status': displays the current VPN connection status and other related information
- 'protonvpn-cli disconnect': disconnects the user from the VPN server
- 'protonvpn-cli logout': logs the user out of their ProtonVPN account
- 'protonvpn-cli refresh': refreshes the user's VPN session token and generates a new session ID
- 'protonvpn-cli config': displays the user's current VPN configuration settings
- 'protonvpn-cli countries': displays a list of available VPN server countries
- 'protonvpn-cli cities': displays a list of available VPN server cities within a specific country

Using the 'protonvpn-cli' tool allows users to manage their ProtonVPN connections and settings with increased efficiency, particularly for those who prefer using command-line interfaces over traditional GUI-based interfaces. 

## tldr 
 
> Official client for ProtonVPN service from the command-line.
> More information: <https://github.com/ProtonVPN/linux-cli>.

- Log in to the ProtonVPN account:

`protonvpn-cli login {{username}}`

- Start a kill switch upon connecting to ProtonVPN:

`protonvpn-cli killswitch --on`

- Connect to ProtonVPN interactively:

`protonvpn-cli connect`

- Display connection status:

`protonvpn-cli status`

- Block malware using ProtonVPN NetShield:

`protonvpn-cli netshield --malware`

- Disconnect from ProtonVPN:

`protonvpn-cli disconnect`

- Display the current ProtonVPN configuration:

`protonvpn-cli config --list`

- Display help for a subcommand:

`protonvpn-cli {{subcommand}} --help`
