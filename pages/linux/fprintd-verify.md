# fprintd-verify 
## chatgpt 
The `fprintd-verify` command is a Linux command-line tool used to verify whether a particular fingerprint matches with the registered fingerprints on the system.

This command is a part of the fprintd tool, which is a fingerprint authentication system that is commonly used in Linux-based operating systems.

The `fprintd-verify` command works by taking a fingerprint sample from the user and comparing it against the registered fingerprints in the system. If the fingerprint matches a registered fingerprint, the verification is successful and the user is granted access.

This command can be particularly useful in securing sensitive data or applications, as fingerprint verification is a reliable way to authenticate users and prevent unauthorized access.

To use the `fprintd-verify` command, you must have a fingerprint scanner installed on your system and registered fingerprints using the fprintd-enroll command. Once you have registered your fingerprints, you can use the `fprintd-verify` command to verify them.

The basic syntax of the `fprintd-verify` command is:

```
fprintd-verify [USER]
```

Where USER is the name of the user whose fingerprint is being verified. If no user is specified, the current user is used by default.

Overall, the `fprintd-verify` command is a simple yet powerful tool for securing your Linux-based system using fingerprint authentication. 

## tldr 
 
> Verify fingerprints against the database.
> More information: <https://manned.org/fprintd-verify>.

- Verify all stored fingerprints for the current user:

`fprintd-verify`

- Verify a specific fingerprint for the current user:

`fprintd-verify --finger {{left-thumb|left-index-finger|left-middle-finger|left-ring-finger|left-little-finger|right-thumb|right-index-finger|right-middle-finger|right-ring-finger|right-little-finger}}`

- Verify fingerprints for a specific user:

`fprint-verify {{username}}`

- Verify a specific fingerprint for a specific user:

`fprintd-verify --finger {{finger_name}} {{username}}`

- Fail the process if a fingerprint doesn't match with ones stored in the database for the current user:

`fprint-verify --g-fatal-warnings`

- Display help:

`fprintd-verify --help`
