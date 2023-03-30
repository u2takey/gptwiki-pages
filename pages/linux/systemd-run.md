# systemd-run 
## chatgpt 
systemd-run is a command that is used to start and manage new system services or user sessions in systemd, a system and service manager for Linux operating systems. 

Syntax: 

The syntax of systemd-run command is as follows:

```systemd-run [OPTIONS] COMMAND [ARGS]```

Here, OPTIONS are the various options that are used with the systemd-run command, COMMAND represents the command to be executed or the service to be started, and ARGS are the arguments passed to the COMMAND.

Options: 

Some of the common options used with systemd-run command are:

- --unit=UNIT_NAME: This option is used to specify the name of the unit under which the service or session should be started. If this option is not provided, systemd-run will automatically generate a unit name based on the command or session name.

- --user: This option is used to start a user session. If this option is not provided, systemd-run will start a system service.

- --scope: This option is used to start a new scope unit that is used to manage processes of a specific type.

- --description=DESCRIPTION: This option is used to provide a description of the service or session.

- --property=PROPERTY: This option is used to set properties for the service or session. Multiple properties can be set using this option.

- --slice=SLICE_NAME: This option is used to specify the slice in which the service or session should be started. If this option is not provided, systemd-run will start the service or session in the default slice.

- --wait: This option is used to wait for the service or session to exit before returning.

- --remain-after-exit: This option is used to keep the service or session running even after the command has exited.

Examples:

1. To start a simple command as a service:

```systemd-run sleep 60```

This command will start the "sleep" command as a service, which will sleep for 60 seconds and then exit.

2. To start a command as a specific service:

```systemd-run --unit=my-service.service sleep 60```

This command will start the "sleep" command as a service with the unit name "my-service.service", which will sleep for 60 seconds and then exit.

3. To start a user session:

```systemd-run --user --description="Test Session"```

This command will start a new user session with the description "Test Session".

4. To start a command in a specific slice:

```systemd-run --slice=my-slice.slice --description="Test Session"```

This command will start a new service in the slice "my-slice.slice" with the description "Test Session". 

## tldr 
 
> Run programs in transient units.
> More information: <https://manned.org/systemd-run>.

- Start a transient service:

`sudo systemd-run {{command}} {{argument1 argument2 ...}}`

- Start a transient service under the service manager of the current user (no privileges):

`systemd-run --user {{command}} {{argument1 argument2 ...}}`

- Start a transient service with a custom unit name and description:

`sudo systemd-run --unit={{name}} --description={{string}} {{command}} {{argument1 argument2 ...}}`

- Start a transient service that does not get cleaned up after it terminates with a custom environment variable:

`sudo systemd-run --remain-after-exit --set-env={{name}}={{value}} {{command}} {{argument1 argument2 ...}}`

- Start a transient timer that periodically runs its transient service (see `man systemd.time` for calendar event format):

`sudo systemd-run --on-calendar={{calendar_event}} {{command}} {{argument1 argument2 ...}}`
