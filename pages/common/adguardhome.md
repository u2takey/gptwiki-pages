# AdGuardHome 
## chatgpt 
AdGuardHome is a command that is used to install and manage AdGuard Home on a server or computer. AdGuard Home is a popular DNS server that blocks ads, trackers, and phishing websites for all devices on a network, providing privacy and security for its users.

To use the AdGuardHome command, you need to first download and install AdGuard Home on your system. Once installed, you can run the command with different parameters to configure and manage various aspects of the AdGuard Home server.

Here are some examples of the AdGuardHome command and their explanations:

1. `adguardhome -h` - This command displays the help menu, which provides information about all the available parameters and options.

2. `adguardhome -d` - This command starts the AdGuard Home server as a background process.

3. `adguardhome -s` - This command stops the AdGuard Home server.

4. `adguardhome -w` - This command launches the AdGuard Home web interface in the system's default web browser.

5. `adguardhome -g` - This command generates a new TLS certificate for AdGuard Home.

6. `adguardhome -r` - This command reloads the AdGuard Home configuration file without stopping the server.

7. `adguardhome -clean` - This command removes the cached DNS records and filters.

Overall, the AdGuardHome command is a useful tool for managing the AdGuard Home DNS server and providing a seamless browsing experience for users on a network. 

## tldr 
 
> A network-wide software for blocking ads & tracking.
> More information: <https://github.com/AdguardTeam/AdGuardHome>.

- Run AdGuard Home:

`AdGuardHome`

- Run AdGuard Home with a specific config:

`AdGuardHome --config {{path/to/AdGuardHome.yaml}}`

- Set the work directory for data to be stored in:

`AdGuardHome --work-dir {{path/to/directory}}`

- Install or uninstall AdGuard Home as a service:

`AdGuardHome --service {{install|uninstall}}`

- Start the AdGuard Home service:

`AdGuardHome --service start`

- Reload the configuration for the AdGuard Home service:

`AdGuardHome --service reload`

- Stop or restart the AdGuard Home service:

`AdGuardHome --service {{stop|restart}}`
