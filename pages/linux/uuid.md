# uuid 
## chatgpt 
`uuid` stands for Universally Unique Identifier. It is a command-line tool that generates a UUID, which is a 128-bit value that is unique across space and time. The generated UUIDs are used to identify objects in a wide range of applications, including computer networking, database management, and software development.

When the `uuid` command is executed, it generates a new UUID and prints it to the standard output. The format of the UUID is a string of 32 hexadecimal digits, separated by hyphens into five groups. The first group contains eight digits, the second and third groups each contain four digits, the fourth group contains three digits, and the final group contains twelve digits.

There are different versions of UUIDs, such as Version 1 (based on the current time and MAC address), Version 2 (based on the current time and a group identifier), and Version 3 and 5 (based on a namespace and a name). By default, the `uuid` command generates a Version 4 UUID, which is based on random numbers.

The `uuid` command can be used in scripts and programs to generate unique identifiers for objects such as files, directories, and processes. It can also be used to generate test data or to generate UUIDs for use in distributed systems. 

## tldr 
 
> Generate and decode Universally Unique Identifiers (UUID).
> See also `uuidgen`.
> More information: <https://manned.org/uuid>.

- Generate a UUIDv1 (based on time and system's hardware address, if present):

`uuid`

- Generate a UUIDv4 (based on random data):

`uuid -v {{4}}`

- Generate multiple UUIDv4 identifiers at once:

`uuid -v {{4}} -n {{number_of_uuids}}`

- Generate a UUIDv4 and specify the output format:

`uuid -v {{4}} -F {{BIN|STR|SIV}}`

- Generate a UUIDv4 and write the output to a file:

`uuid -v {{4}} -o {{path/to/file}}`

- Generate a UUIDv5 (based on the supplied object name) with a specified namespace prefix:

`uuid -v {{5}} ns:{{DNS|URL|OID|X500}} {{object_name}}`

- Decode a given UUID:

`uuid -d {{uuid}}`
