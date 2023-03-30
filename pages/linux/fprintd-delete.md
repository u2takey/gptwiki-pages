# fprintd-delete 
## chatgpt 
The command "fprintd-delete" is used to delete a registered fingerprint from the system's fingerprint database. 

- "fprintd" refers to the Fingerprint Daemon, a service that runs in the background to handle fingerprint-related tasks on Linux systems. 
- "_delete" specifies the action that will be performed, which is the deletion of a fingerprint.

When you run the "fprintd-delete" command, you will need to provide the ID of the fingerprint you want to delete. To obtain the ID, you can use the "fprintd-list" command to list all registered fingerprints.

Note that you will need administrative privileges (sudo access) to run "fprintd-delete" because modifying the fingerprint database requires elevated privileges. 

Example usage: 

$ sudo fprintd-delete -u user1 1

This command will delete fingerprint ID 1 from the database of the user 'user1'. 

## tldr 
 
> Remove fingerprints from the database.
> More information: <https://manned.org/fprintd-delete>.

- Remove all fingerprints for a specific user:

`fprintd-delete {{username}}`

- Remove a specific fingerprints for a specific user:

`fprintd-delete {{username}} --finger {{left-thumb|left-index-finger|left-middle-finger|left-ring-finger|left-little-finger|right-thumb|right-index-finger|right-middle-finger|right-ring-finger|right-little-finger}}`

- Display help:

`fprintd-delete`
