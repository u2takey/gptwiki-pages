# ubuntu-security-status 
## chatgpt 
The "ubuntu-security-status" command is used to display information about the security status of the Ubuntu system. 

When this command is executed, it generates a report that shows the status of the system in terms of security updates that are available or need to be installed. The report includes the following information:

1. Number of security updates that are available for the system
2. Number of security updates that need to be installed
3. Information about the security release that the system is running on
4. List of packages that have security updates available
5. List of packages that have security updates installed

This command can be useful in determining the security status of an Ubuntu system, and for identifying any packages that need to be updated to address security vulnerabilities. It should be executed periodically to ensure that the system is up to date with the latest security patches.

Overall, the "ubuntu-security-status" command is a simple and effective way to perform a security audit of an Ubuntu system. 

## tldr 
 
> Display information about security support for installed Ubuntu packages.
> More information: <https://git.launchpad.net/ubuntu/+source/update-manager/tree/ubuntu-security-status>.

- Display the number of unsupported packages:

`ubuntu-security-status`

- List packages that are no longer available for download:

`ubuntu-security-status --unavailable`

- List third-party packages:

`ubuntu-security-status --thirdparty`
