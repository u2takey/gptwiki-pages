# clamdscan 
## chatgpt 
clamdscan is a command-line tool used to scan files and directories for viruses and malware using the ClamAV antivirus engine. ClamAV is an open-source antivirus software that is designed to detect various types of malicious software, including viruses, trojans, worms, and other malware.

When you run the "clamdscan" command, ClamAV will start scanning your specified files and directories for infections. You can configure the tool to scan specific file types or exclude certain directories from the scan. You can also use various options and flags to customize your scan.

Here is the basic syntax for using the "clamdscan" command:

```
clamdscan [options] [file or directory]
```

Options:
- -h: Shows help on how to use clamdscan.
- -v: Shows the version of ClamAV.
- -m: Only prints infected files.
- -r: Scans directories recursively.


Example:
To scan a directory recursively, use the following command:
```
clamdscan -r /home/user/Documents/
```

This command will scan all files and subdirectories in the "/home/user/Documents/" directory, and print any infected files it finds.

In summary, clamdscan is a powerful command-line tool for scanning files and directories for viruses and malware. It's an essential tool for any system administrator or security professional who needs to protect their network from cyber threats. 

## tldr 
 
> A command-line virus scanner using the ClamAV Daemon.
> More information: <https://www.clamav.net>.

- Scan a file or directory for vulnerabilities:

`clamdscan {{path/to/file_or_directory}}`

- Scan data from `stdin`:

`{{command}} | clamdscan -`

- Scan the current directory and output only infected files:

`clamdscan --infected`

- Output the scan report to a log file:

`clamdscan --log {{path/to/log_file}}`

- Move infected files to a specific directory:

`clamdscan --move {{path/to/quarantine_directory}}`

- Remove infected files:

`clamdscan --remove`

- Use multiple threads to scan a directory:

`clamdscan --multiscan`

- Pass the file descriptor instead of streaming the file to the daemon:

`clamdscan --fdpass`
