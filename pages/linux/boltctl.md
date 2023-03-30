# boltctl 
## chatgpt 
The `boltctl` command is used to manage the Thunderbolt devices (such as docks, external GPUs) attached to a computer. This command allows users to perform various tasks and operations related to Thunderbolt devices. Here are some of the tasks that can be performed using `boltctl`:

1. Listing Thunderbolt devices: The command `boltctl list` can be used to list all connected Thunderbolt devices.

2. Enabling and disabling device security: With `boltctl security`, users can enable or disable device security policies set in the Thunderbolt firmware.

3. Authorizing devices: One can authorize a device using the command `boltctl authorize <device_id>`. This allows the device to be used automatically in the future without needing a password.

4. Revoking authorization: The command `boltctl unauthorize <device_id>` can be used to remove device authorization.

5. Showing details about a device: One can use `boltctl details <device_id>` to show details about a specific Thunderbolt device.

6. Power management: One can turn off a Thunderbolt device using `boltctl power off <device_id>` command, and on using `boltctl power on <device_id>`.

These are just a few examples of what can be done using the `boltctl` command. In summary, `boltctl` is a command-line tool designed for managing Thunderbolt devices on Linux operating systems. 

## tldr 
 
> Control thunderbolt devices.
> More information: <https://manned.org/boltctl>.

- List connected (and authorized) devices:

`boltctl`

- List connected devices, including unauthorized ones:

`boltctl list`

- Authorize a device temporarily:

`boltctl authorize {{device_uuid}}`

- Authorize and remember a device:

`boltctl enroll {{device_uuid}}`

- Revoke a previously authorized device:

`boltctl forget {{device_uuid}}`

- Show more information about a device:

`boltctl info {{device_uuid}}`
