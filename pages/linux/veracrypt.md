# veracrypt 
## chatgpt 
Veracrypt is a command used for encryption and decryption of files and volumes. The command is used to create and manage encrypted volumes on the user’s computer. 

The veracrypt command offers a variety of options that allow users to perform tasks such as creating new encrypted volumes, mounting existing volumes, changing passwords, and generating rescue disks for recovery purposes.

The veracrypt command has syntax that includes specifying the volume to be encrypted, the encryption algorithm to be used, and specifying the mount point for the encrypted volume.

Examples of commonly used options with the veracrypt command include:

-‘–create’ option to create a new encrypted volume
-‘–volume’ option to specify the volume to be encrypted
-‘–password’ option to specify the password to be used to encrypt the volume
-‘–mount’ option to specify the mount point for the encrypted volume

Overall, the veracrypt command is a powerful tool for encrypting sensitive information on a computer and protecting it from unauthorized access. 

## tldr 
 
> Free and open source disk encryption software.
> More information: <https://www.veracrypt.fr/code/VeraCrypt/plain/doc/html/Documentation.html>.

- Create a new volume through a text user interface and use `/dev/urandom` as a source of random data:

`veracrypt --text --create --random-source={{/dev/urandom}}`

- Decrypt a volume interactively through a text user interface and mount it to a directory:

`veracrypt --text {{path/to/volume}} {{path/to/mount_point}}`

- Decrypt a partition using a keyfile and mount it to a directory:

`veracrypt --keyfiles={{path/to/keyfile}} {{/dev/sdXN}} {{path/to/mount_point}}`

- Dismount a volume on the directory it is mounted to:

`veracrypt --dismount {{path/to/mounted_point}}`
