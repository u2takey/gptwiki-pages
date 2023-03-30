# nmtui 
## chatgpt 
nmtui is a command line utility that allows users to manage network connections using a user-friendly text-based interface. 

When you type "nmtui" command in the terminal, it launches a text-based user interface that allows you to perform a number of network-related tasks such as create, connect, modify, delete, and configure network devices, change networking settings, and configure DNS settings.

Once you are in the nmtui interface, you can use the arrow keys to navigate the different options and select the appropriate option for your needs. For example, if you want to connect to a network, you can select "Activate a connection" and choose the network you want to connect to from the list of available networks.

Overall, nmtui is a convenient and efficient way to manage network connections and settings on Linux systems without requiring extensive command-line knowledge. 

## tldr 
 
> Text user interface for controlling NetworkManager.
> Use arrow keys to navigate, enter to select an option.
> More information: <https://networkmanager.dev/docs/api/latest/nmtui.html>.

- Open the user interface:

`nmtui`

- Show a list of available connections, with the option to activate or deactivate them:

`nmtui connect`

- Connect to a given network:

`nmtui connect {{name|uuid|device|SSID}}`

- Edit/Add/Delete a given network:

`nmtui edit {{name|id}}`

- Set the system hostname:

`nmtui hostname`
