# syncthing 
## chatgpt 
Syncthing is a command line tool that is used for file synchronization between multiple devices. It allows users to keep their data synchronized across devices in real-time, which can be useful for remote teams working on the same project, or for individuals who need to access their files on multiple devices.

To use Syncthing, users first need to install it on each device they want to synchronize. Once installed, they can set up folders that they want to sync between the devices, either on their own or in collaboration with other Syncthing users.

The command line syntax for using Syncthing depends on the specific task the user wants to perform. For example, to install Syncthing on a Linux system using the command line, the user would need to:

1. Add the Syncthing repository to their system’s package manager.
2. Update the package manager.
3. Install Syncthing using the package manager command.

Once installed, users can use the Syncthing command line interface to manage their synced folders, check the status of their synchronization, and view detailed logs of the sync process. They can also use the Syncthing web interface to access more advanced settings and features, including configuring devices to connect over the internet, setting up encryption, and creating advanced folder synchronization rules. 

## tldr 
 
> Continuous bidirectional decentralised folder synchronisation tool.
> More information: <https://docs.syncthing.net/>.

- Start Syncthing:

`syncthing`

- Start Syncthing without opening a web browser:

`syncthing -no-browser`

- Print the device ID:

`syncthing -device-id`

- Change the home directory:

`syncthing -home={{path/to/directory}}`

- Force a full index exchange:

`syncthing -reset-deltas`

- Change the address upon which the web interface listens:

`syncthing -gui-address={{ip_address:port|path/to/socket.sock}}`

- Show filepaths to the files used by Syncthing:

`syncthing -paths`

- Disable the Syncthing monitor process:

`syncthing -no-restart`
