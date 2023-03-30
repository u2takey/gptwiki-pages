# fwupdmgr 
## chatgpt 
fwupdmgr is a command-line tool used to manage firmware updates on Linux systems. It is typically used to update firmware on devices such as BIOS, hard drives, SSDs, network interfaces, and others. Here are some of the commonly used options with fwupdmgr:

1. `fwupdmgr get-devices`: This command displays the list of devices that can be updated with fwupdmgr.

2. `fwupdmgr get-updates`: This command shows the available updates for the devices that can be updated with fwupdmgr.

3. `fwupdmgr update`: This command downloads and installs the available updates.

4. `fwupdmgr install <filename>`: This command installs a firmware update from a local file.

5. `fwupdmgr disable <fwupdmgr-plugin>`: This command disables a fwupdmgr plugin which prevents it from updating firmware.

6. `fwupdmgr enable <fwupdmgr-plugin>`: This command enables a fwupdmgr plugin which allows it to update firmware.

Overall, fwupdmgr is a powerful tool for managing firmware updates on Linux systems. It is important to use the tool carefully and ensure that the firmware updates are done correctly to avoid any issues with the system. 

## tldr 
 
> A tool for updating device firmware, including UEFI, using `fwupd`.
> More information: <https://fwupd.org/>.

- Display all devices detected by fwupd:

`fwupdmgr get-devices`

- Download the latest firmware metadata from LVFS:

`fwupdmgr refresh`

- List the updates available for devices on your system:

`fwupdmgr get-updates`

- Install firmware updates:

`fwupdmgr update`
