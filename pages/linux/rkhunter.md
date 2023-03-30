# rkhunter 
## chatgpt 
Rkhunter stands for Rootkit Hunter. It is a command-line utility used for system scan, detection, and removal of rootkits, backdoors, and other security threats on Linux and other Unix-like systems.

The rkhunter command works by comparing the output of the core system files against known database signatures of known rootkits and malware. If it detects any inconsistencies, it reports it to the user.

The rkhunter tool also performs a number of other security checks on the system, such as checking for suspicious files, open ports, and user accounts. It also checks for known vulnerabilities in the installed software and warns the user about them.

To use the rkhunter command, open a terminal and run the command with superuser privileges:

```
sudo rkhunter --check
```

This will initiate a scan of your system for rootkits and other security threats. Make sure to update the rkhunter database signatures regularly by running:

```
sudo rkhunter --update
```

Overall, using the rkhunter command regularly helps to enhance the security and integrity of your Linux system by keeping it free from malicious threats. 

## tldr 
 
> Searches for rootkits and malware.
> More information: <https://wiki.archlinux.org/title/Rkhunter>.

- Check a system for rootkits and malware:

`sudo rkhunter --check`

- Update rkhunter:

`sudo rkhunter --update`

- Print all available tests:

`sudo rkhunter --list`

- Display version:

`sudo rkhunter --versioncheck`

- Display help:

`sudo rkhunter --help`
