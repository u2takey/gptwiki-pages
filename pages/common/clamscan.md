# clamscan 
## chatgpt 
The "clamscan" command is a Linux command used to scan files, directories, and entire file systems for malware and viruses using the ClamAV antivirus software. When used, it will initiate a scan and return the results of the scan.

Here is how to use "clamscan" command:

1. Open the terminal on your Linux operating system.

2. Type "clamscan" followed by the path to the file or directory you want to scan. For example, if you want to scan your home directory, you can enter the following command: clamscan ~

3. Hit "Enter" and the scan will begin. Depending on the size of the file or directory, the scan may take some time to complete.

4. After the scan is complete, "clamscan" will generate a report of the scan results, indicating whether any malware or viruses were found.

It's important to note that "clamscan" is a command-line tool and does not have a graphical user interface. It's recommended for advanced users who are familiar with the command line and Linux operating system. 

## tldr 
 
> A command-line virus scanner.
> More information: <https://www.clamav.net>.

- Scan a file for vulnerabilities:

`clamscan {{path/to/file}}`

- Scan all files recursively in a specific directory:

`clamscan -r {{path/to/directory}}`

- Scan data from `stdin`:

`{{command}} | clamscan -`

- Specify a virus database file or directory of files:

`clamscan --database {{path/to/database_file_or_directory}}`

- Scan the current directory and output only infected files:

`clamscan --infected`

- Output the scan report to a log file:

`clamscan --log {{path/to/log_file}}`

- Move infected files to a specific directory:

`clamscan --move {{path/to/quarantine_directory}}`

- Remove infected files:

`clamscan --remove yes`
