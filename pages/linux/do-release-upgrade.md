# do-release-upgrade 
## chatgpt 
The `do-release-upgrade` command is a Linux terminal command used to upgrade an Ubuntu system to the latest version of Ubuntu available. This command is used to perform a system upgrade to a newer release, and it is typically used when a new Ubuntu version is available.

When this command is executed, it will check to see if there is a new version of Ubuntu available. It will then download all the necessary files and packages required to upgrade the system, and then it will initiate the upgrade process. During the upgrade process, the old Ubuntu version is replaced with the new version, and all the system configurations and settings are transferred to the new version.

It is important to note that running `do-release-upgrade` can take some time, depending on the speed of your internet connection and the size of the updates being installed. It is recommended that you backup your important files and data before running this command, in case anything unexpected happens during the upgrade process.

Overall, the `do-release-upgrade` command is a convenient way to upgrade your Ubuntu system to the latest version without having to reinstall your operating system from scratch. 

## tldr 
 
> The Ubuntu release upgrader.
> More information: <https://ubuntu.com/server/docs/upgrade-introduction>.

- Upgrade to the latest release:

`sudo do-release-upgrade`

- Upgrade to the latest development release:

`sudo do-release-upgrade --devel-release`

- Upgrade to the latest proposed release:

`sudo do-release-upgrade --proposed`
