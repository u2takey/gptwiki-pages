# gnmic set 
## chatgpt 
The "gnmic set" command is a command-line tool used for managing network devices and systems through the gRPC Network Management Interface (gNMI) protocol. It allows users to set the values of various parameters and attributes within network devices and systems.

The command syntax is as follows:

```
gnmic set <options> <targets> <path value pairs>
```

- The "options" field specifies any additional options to be used with the command, such as authentication or logging options.
- The "targets" field specifies the network devices or systems that the command will apply to.
- The "path value pairs" field specifies the specific parameters or attributes and their corresponding values that are being set.

For example, the following command sets the description of a network interface on a device:

```
gnmic set -target=myrouter01:57400 -username=admin -password='password' /interfaces/interface[name=eth0]/description='New description'
```

Here, the "target" option specifies the device and the "username" and "password" options provide login credentials. The "path value pairs" options specify the interface named "eth0" and set its description to "New description."

Overall, the "gnmic set" command is a powerful tool for managing network devices and systems through the gNMI protocol, allowing for automation and quick updates to configurations. 

## tldr 
 
> Modify gnmi network device configuration.
> More information: <https://gnmic.kmrd.dev/cmd/set>.

- Update the value of a path:

`gnmic --address {{ip:port}} set --update-path {{path}} --update-value {{value}}`

- Update the value of a path to match the contents of a json file:

`gnmic -a {{ip:port}} set --update-path {{path}} --update-file {{filepath}}`

- Replace the value of a path to match the contents of a json file:

`gnmic -a {{ip:port}} set --replace-path {{path}} --replace-file {{filepath}}`

- Delete the node at a given path:

`gnmic -a {{ip:port}} set --delete {{path}}`
