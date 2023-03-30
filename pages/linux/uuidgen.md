# uuidgen 
## chatgpt 
The `uuidgen` command generates a universal unique identifier (UUID), also known as a GUID, that is a 128-bit value typically represented as a string of 36 characters. A UUID is a standardized identifier that is unique across all systems and has very low probability of collision with other UUIDs.

When you run the `uuidgen` command in a terminal or command prompt, it will generate a new UUID and display it on the screen. The exact format of the UUID depends on the operating system and version of the `uuidgen` command being used.

UUIDs can be useful for identifying objects or entities in computer systems where uniqueness is important, such as in distributed systems, databases, or file systems. Examples of where UUIDs are used include identifying unique devices, creating unique session identifiers for web applications, and generating random encryption keys.

Overall, `uuidgen` is a simple but powerful command that can be useful in a wide range of programming and systems administration tasks where unique identifiers are needed. 

## tldr 
 
> Generate unique identifiers (UUIDs).
> See also `uuid`.
> More information: <https://manned.org/uuidgen>.

- Create a random UUIDv4:

`uuidgen --random`

- Create a UUIDv1 based on the current time:

`uuidgen --time`

- Create a UUIDv5 of the name with a specified namespace prefix:

`uuidgen --sha1 --namespace {{@dns|@url|@oid|@x500}} --name {{object_name}}`
