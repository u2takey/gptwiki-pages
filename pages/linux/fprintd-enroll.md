# fprintd-enroll 
## chatgpt 
The "fprintd-enroll" command is a Linux command used for enrolling fingerprints for authentication purposes. It is a command-line utility that interacts with the fprintd service, which is a fingerprint authentication service used on Linux systems. 

The "enroll" in the command refers to the process of capturing a user's fingerprint and storing it in the system's database for future authentication. The fprintd-enroll utility captures fingerprint data from the user's fingerprint reader and stores it in a directory within the user's home folder.

When executed, the fprintd-enroll command initiates the enrollment process by communicating with the fprintd service. The user is prompted to place their finger on the fingerprint reader so that it can be scanned and stored in the system's authentication database.

The fingerprint data is then encrypted and stored in a secure location on the system. Once the enrollment process is complete, the user will be able to use their fingerprint as an authentication method for login, password prompts or other authentication requests.

In summary, "fprintd-enroll" is a Linux command that allows users to enroll their fingerprints for use as an authentication method. It interacts with the fprintd service and captures fingerprint data from the user's fingerprint reader, encrypts it and stores it in a secure location on the system. 

## tldr 
 
> Enroll fingerprints into the database.
> More information: <https://manned.org/fprintd-enroll>.

- Enroll the right index finger for the current user:

`fprintd-enroll`

- Enroll a specific finger for the current user:

`fprintd-enroll --finger {{left-thumb|left-index-finger|left-middle-finger|left-ring-finger|left-little-finger|right-thumb|right-index-finger|right-middle-finger|right-ring-finger|right-little-finger}}`

- Enroll the right index finger for a specific user:

`fprintd-enroll {{username}}`

- Enroll a specific finger for a specific user:

`fprintd-enroll --finger {{finger_name}} {{username}}`

- Display help:

`fprintd-enroll --help`
