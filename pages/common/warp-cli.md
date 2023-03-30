# warp-cli 
## chatgpt 
The warp-cli command is a command line tool used to manage and configure Cloudflare's WARP VPN. When executed, the command provides a set of options and subcommands that allows you to perform various tasks related to WARP configuration and management. Some of the common subcommands provided by the warp-cli command include:

1. `connect`: This subcommand is used to connect your device to the WARP VPN.

2. `disconnect`: This subcommand is used to disconnect your device from the WARP VPN.

3. `register`: This subcommand is used to register a new device with the WARP VPN.

4. `status`: This subcommand is used to check the status of your WARP VPN connection.

5. `account`: This subcommand is used to manage your Cloudflare account settings, such as updating your email address or password.

6. `version`: This subcommand is used to check the version of the WARP CLI tool.

To use the warp-cli command, you need to have it installed on your device and must have an active subscription to the Cloudflare WARP VPN service. Once you have installed the command, you can run it from the command line interface (CLI) of your operating system. 

## tldr 
 
> Official command-line client for Cloudflare's WARP service.
> More information: <https://developers.cloudflare.com/warp-client/>.

- Register the current device to WARP (must be run before first connection):

`warp-cli register`

- Connect to WARP:

`warp-cli connect`

- Disconnect from WARP:

`warp-cli disconnect`

- Display the WARP connection status:

`warp-cli status`

- Display help:

`warp-cli help`

- Display help for a subcommand:

`warp-cli help {{subcommand}}`
