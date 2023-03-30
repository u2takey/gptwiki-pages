# synoupgrade 
## chatgpt 
As an AI language model, I do not have access to specific software or systems installed on your computer or server. However, based on my research and general knowledge of the term, here is a tentative explanation of the "synoupgrade" command:

Synoupgrade is a command line utility typically used in Synology's DiskStation Manager (DSM) operating system. It is a package manager that can be used to install, upgrade, or manage packages and applications on a Synology NAS (Network Attached Storage) device. The DSM operating system comes with a wide variety of packages and applications that can be downloaded and installed via Synoupgrade, which can enhance the functionality of a Synology NAS. 

When Synoupgrade command is run, it typically checks the Synology package sources to identify any available updates to installed packages and applications. It then downloads and installs the latest version of the packages or applications, updating the system software and improving stability, security, compatibility, and performance. Synoupgrade command ensures that the Synology NAS device is always running the latest and most secure version of the installed packages and applications.

The specific syntax and parameters of the Synoupgrade command may vary depending on the version and configuration of Synology DSM installed on the device. Users are advised to consult the DSM user manual or built-in help documentation for more information on using Synoupgrade command.  Overall, Synoupgrade is a valuable command used to keep the Synology NAS system software up-to-date, secure and optimised. 

## tldr 
 
> Upgrade a Synology DiskStation Manager (DSM) from the command-line.
> More information: <https://www.synology.com/dsm>.

- Check if upgrades are available:

`sudo synoupgrade --check`

- Check for patches without upgrading the DSM version:

`sudo synoupgrade --check-smallupdate`

- Download the latest upgrade available (use `--download-smallupdate` for patches):

`sudo synoupgrade --download`

- Start the upgrade process:

`sudo synoupgrade --start`

- Upgrade to the latest version automatically:

`sudo synoupgrade --auto`

- Apply patches without upgrading the DSM version automatically:

`sudo synoupgrade --auto-smallupdate`

- Upgrade the DSM using a patch file (should be an absolute path):

`sudo synoupgrade --patch {{/path/to/file.pat}}`

- Display help:

`synoupgrade`
