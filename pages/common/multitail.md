# multitail 
## chatgpt 
Multitail is a command-line utility that allows multiple log files to be viewed simultaneously in a single terminal window. It is commonly used by system administrators and software developers to monitor log files in real-time, and to quickly identify issues or errors that may occur.

Here is a brief overview of how the multitail command works:

1. Install multitail: If multitail is not already installed on your system, you will need to install it first.

2. Specify one or more log file(s): Next, use the multitail command to specify which log file(s) you want to monitor. For example, to monitor the Apache access and error logs, you could run:

```
multitail /var/log/apache2/access.log /var/log/apache2/error.log
```

3. Customize the display: You can customize the output of multitail by using various options and flags. For example, you can specify the colors used for different types of log entries, set the refresh interval, and adjust the layout of the output.

4. View the logs: Once you have configured multitail to your liking, you can start monitoring the logs in real-time. The tool will display new log entries as they are added to the file(s), and highlight any entries that match your custom settings.

Overall, multitail is a useful tool for monitoring multiple log files at once, and can help you quickly identify problems and troubleshoot issues with your system or applications. 

## tldr 
 
> Extension of tail.
> More information: <https://manned.org/multitail>.

- Tail all files matching a pattern in a single stream:

`multitail -Q 1 '{{pattern}}'`

- Tail all files in a directory in a single stream:

`multitail -Q 1 '{{path/to/directory}}/*'`

- Automatically add new files to a window:

`multitail -Q {{pattern}}`

- Show 5 logfiles while merging 2 and put them in 2 columns with only one in the left column:

`multitail -s 2 -sn 1,3 {{mergefile}} -I {{file1}} {{file2}} {{file3}} {{file4}}`
