# particle 
## chatgpt 
Particle is a command-line interface tool used to interact with Particle devices and services. It allows developers and users to send commands, retrieve information, and manage devices remotely through the Particle Cloud.

The primary command to use Particle is the "particle" command itself, which can be used for various tasks like logging in, creating and managing devices, and interacting with device functions.

Some of the most common commands used with Particle are:

1. particle login: This command is used to log in to the Particle Cloud, which provides access to all Particle devices and services.

2. particle list: This command is used to list all the devices associated with the user's account.

3. particle device add: This command is used to add a new device to the user's account.

4. particle device remove: This command is used to remove an existing device from the user's account.

5. particle device rename: This command is used to rename an existing device.

6. particle call: This command is used to invoke a function on a device.

7. particle publish: This command is used to publish events to the Particle Cloud.

8. particle serial identify: This command is used to identify a device connected to the computer via serial port.

These are some of the most commonly used commands with Particle, but there are many more available depending on the use case. Particle is a powerful tool for developers and users alike, offering a simple and intuitive way to interact with Particle devices and services. 

## tldr 
 
> A command-line tool for interacting with Particle devices.
> More information: <https://docs.particle.io/tutorials/developer-tools/cli>.

- Log in or create an account for the Particle CLI:

`particle setup`

- Display a list of devices:

`particle list`

- Create a new Particle project interactively:

`particle project create`

- Compile a Particle project:

`particle compile {{device_type}} {{path/to/source_code.ino}}`

- Update a device to use a specific app remotely:

`particle flash {{device_name}} {{path/to/program.bin}}`

- Update a device to use the latest firmware via serial:

`particle flash --serial {{path/to/firmware.bin}}`

- Execute a function on a device:

`particle call {{device_name}} {{function_name}} {{function_arguments}}`
