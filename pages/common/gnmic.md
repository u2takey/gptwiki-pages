# gnmic 
## chatgpt 
gnmic is a command-line interface (CLI) tool for interacting with network devices using the gNMI (gRPC Network Management Interface) protocol. The gNMI protocol is a standard interface for network management and telemetry that uses gRPC (a high-performance, open-source framework for remote procedure calls) as its underlying communication mechanism.

The gnmic command is used to perform various network management tasks, such as retrieving configuration and operational data from network devices, setting or changing the configuration of network devices, subscribing to streaming telemetry data from network devices, and more. To use gnmic, you need to have a gNMI-enabled network device and the necessary access credentials to communicate with it.

Here are some examples of gnmic commands:

- gnmic get - Retrieves the configuration or operational data from a network device.
- gnmic set - Sets or changes the configuration of a network device.
- gnmic subscribe - Subscribes to streaming telemetry data from a network device.
- gnmic cap - Retrieves the gNMI capabilities of a network device.
- gnmic version - Displays the current version of the gnmic client.

Overall, gnmic is a powerful tool for network management and telemetry, and it provides a simple and consistent way to interact with network devices that support the gNMI protocol. 

## tldr 
 
> A gNMI command-line client.
> Manage gNMI network device configuration and view operational data.
> More information: <https://gnmic.kmrd.dev>.

- Request device capabilities:

`gnmic --address {{ip:port}} capabilities`

- Provide a username and password to fetch device capabilities:

`gnmic --address {{ip:port}} --username {{username}} --password {{password}} capabilities`

- Get a snapshot of the device state at a specific path:

`gnmic -a {{ip:port}} get --path {{path}}`

- Update device state at a specific path:

`gnmic -a {{ip:port}} set --update-path {{path}} --update-value {{value}}`

- Subscribe to target state updates under the subtree at a specific path:

`gnmic -a {{ip:port}} subscribe --path {{path}}`
