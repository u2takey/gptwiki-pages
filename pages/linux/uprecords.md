# uprecords 
## chatgpt 
The `uprecords` command is used to display a list of the uptime records of a system. When a system is running continuously without any shutdowns or reboots, its uptime is continuously increasing.

The `uprecords` command retrieves the system’s uptime history and displays it in a tabulated format. The tabulated format of the output consists of the following columns:

1. **Nr** - The record number of the displayed uptime.
2. **Uptime** - The total time the system has been running since the last reboot or system startup.
3. **Date** - The date and time when the system was last started or rebooted.
4. **Since\_time** - The time when the system was last started or rebooted.

By default, the `uprecords` command displays the last ten records. However, you can change the number of records displayed by specifying the number as an argument on the command line.

For example, to display the last 20 records of uptime, you would enter the following command: 

```
uprecords 20
```

Overall, the `uprecords` command is a simple but helpful utility for tracking system uptime and system uptime history. 

## tldr 
 
> Displays a summary of historical uptime records.
> More information: <https://manned.org/uprecords>.

- Display a summary of the top 10 historical uptime records:

`uprecords`

- Display the top 25 records:

`uprecords -m {{25}}`

- Display the downtime between reboots instead of the kernel version:

`uprecords -d`

- Show the most recent reboots:

`uprecords -B`

- Don't truncate information:

`uprecords -w`
