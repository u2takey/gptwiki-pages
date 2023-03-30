# fprintd-list 
## chatgpt 
The "fprintd-list" command is used to list all the enrolled fingerprints on the system. This command is used in Linux-based operating systems and requires administrative privileges to execute.

When this command is run, it communicates with the Fingerprint Authentication Daemon (fprintd) which is responsible for managing and authenticating fingerprints. The daemon retrieves the list of enrolled fingerprints from the system and displays them in the terminal.

The output of the "fprintd-list" command includes the name of the device or user account that the fingerprint is associated with, the corresponding finger that was used to enroll the fingerprint, and the unique identifier for the fingerprint.

This command is useful for system administrators who need to manage fingerprints enrolled on the system. They can use it to check if a particular user has enrolled a fingerprint or to remove outdated fingerprints from the system. 

## tldr 
 
> List enrolled fingerprints.
> More information: <https://manned.org/fprintd-list>.

- List enrolled fingerprints for a specific user:

`fprintd-list {{username}}`

- List enrolled fingerprints for a space-separated list of users:

`fprintd-list {{username1 username2 ...}}`

- Display help:

`fprintd-list`
