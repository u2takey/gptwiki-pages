# fprintd 
## chatgpt 
fprintd is a command-line tool used to manage fingerprints on a system. It is a part of the fprint project, which is an open-source project that provides support for fingerprint readers on Linux systems.

The fprintd command is used to interact with the fingerprint daemon, which is responsible for managing the fingerprint reader device and storing fingerprint data. With fprintd, you can enroll new fingerprints, remove existing fingerprints, and manage authentication settings.

Here are some common examples of using fprintd:

- `fprintd-enroll`: This command is used to enroll a new fingerprint. When you run this command, you will be prompted to scan your finger several times to create a fingerprint template. You can optionally specify a label for the fingerprint to help identify it later.
- `fprintd-delete`: This command is used to remove a fingerprint. You need to specify the label or the index number of the fingerprint you want to remove.
- `fprintd-list`: This command is used to list all the enrolled fingerprints on the system. It will display the label and index number of each fingerprint.
- `fprintd-verify`: This command is used to verify a fingerprint. You will be prompted to scan your finger, and if the fingerprint matches a stored template, you will be authenticated.

Overall, fprintd is a useful tool for managing fingerprints on Linux systems that have a fingerprint reader device. 

## tldr 
 
> Fingerprint management daemon.
> More information: <https://fprint.freedesktop.org/>.

- Display the man page for `fprintd`:

`man fprintd`
