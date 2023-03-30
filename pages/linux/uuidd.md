# uuidd 
## chatgpt 
The `uuidd` command is used in Unix and Unix-like operating systems to generate and manage UUIDs (Universally Unique Identifiers).

UUIDs are unique 128-bit identifiers that are commonly used in computer systems to identify objects and entities such as network interfaces, files, and processes. They are generated using algorithms that take into account various unique factors such as the computer's MAC address, the time since the system was started, and random numbers.

The `uuidd` service is responsible for managing the UUIDs in the system. When the service is started, it generates a pool of UUIDs and stores them in memory. When a program requests a UUID, the `uuidd` service retrieves one from the pool and returns it to the program.

The `uuidd` command can be used to control and customize the `uuidd` service. Some common options and subcommands include:

- `-d`: Run `uuidd` in debug mode.
- `-f`: Run `uuidd` in the foreground.
- `-k`: Kill the current `uuidd` process.
- `-p`: Print the current pool of UUIDs.
- `-s`: Set the size of the UUID pool. By default, the pool size is 1024.
- `-t`: Set the timeout for UUIDs. By default, UUIDs will expire after 60 seconds.
- `reload`: Reload the configuration files for `uuidd`.
- `restart`: Stop and then start the `uuidd` service.
- `start`: Start the `uuidd` service.
- `status`: Check the status of the `uuidd` service.
- `stop`: Stop the `uuidd` service.

Overall, the `uuidd` command is an essential tool for managing UUIDs in Unix and Unix-like systems. 

## tldr 
 
> Daemon for generating UUIDs.
> More information: <https://manned.org/uuidd>.

- Generate a random UUID:

`uuidd --random`

- Generate a bulk number of random UUIDs:

`uuidd --random --uuids {{number_of_uuids}}`

- Generate a time-based UUID, based on the current time and MAC address of the system:

`uuidd --time`
