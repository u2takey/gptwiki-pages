# pio update 
## chatgpt 
`pio update` is a command used in PlatformIO, an open-source ecosystem for embedded development. 

The command is used to update the PlatformIO development environment, including platform development frameworks, libraries, and tools, to the latest versions available. It helps to ensure that developers are using the most up-to-date and stable versions of all components in their development projects.

When you run the `pio update` command, PlatformIO checks for available updates for your installed platforms, frameworks, libraries, and tools. If there are any available updates, the system will download and install them automatically. The update process is carried out through the internet and might take a while, depending on the size of the updates.

Overall, the `pio update` command is an essential command used in PlatformIO to keep developers' development environment up-to-date and ensure that they have access to the latest features and capabilities in their projects. 

## tldr 
 
> Update installed PlatformIO Core packages, development platforms and global libraries.
> See also: `pio platform update`, `pio lib update`.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_update.html>.

- Perform a full update of all packages, development platforms and global libraries:

`pio update`

- Update core packages only (skips platforms and libraries):

`pio update --core-packages`

- Check for new versions of packages, platforms and libraries but do not actually update them:

`pio update --dry-run`
