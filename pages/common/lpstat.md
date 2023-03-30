# lpstat 
## chatgpt 
The 'lpstat' command in Linux is used to check the status of print jobs that are in the print queue, print status of printers and print servers, and configuration information. The lpstat command is used to display information about print queues and printer status.

Syntax:

The syntax of lpstat command is as follows:

$ lpstat [ -a ] [ -c ] [ -h server[:port] ] [ -p [destinations] ] [ -r ] [ -s ] [ -t ] [ -u [users] ]

Options:

-a : Prints status of all the print queues.

-c : Prints the classes of printers.

-h server[:port] : Specified the hostname and port of the printer server.

-p [destinations] : Prints the status of only the specified printers or destinations.

-r : Prints the default system printer.

-s : Prints only the status of the printer queue.

-t : Prints the status of all printers attached.

-u [users] : Prints the status of jobs that belong to the specified users.

Examples:

1. To show all available printer queues on the system, use the command:

$ lpstat -a

2. To show the printer status of a particular printer, use the command:

$ lpstat -p lp1

3. To check the status of print jobs that belong to a specific user, use the command:

$ lpstat -u john

4. To list all the active print jobs on your system use the command:

$ lpstat -t

5. To list the printers and their details that are configured on the system, use the command:

$ lpstat -v

These are some of the examples of how the 'lpstat' command can be used to check the printer status and job statuses. 

## tldr 
 
> Show status information about printers.
> More information: <https://manned.org/lpstat>.

- List printers present on the machine and whether they are enabled for printing:

`lpstat -p`

- Show the default printer:

`lpstat -d`

- Display all available status information:

`lpstat -t`

- Show a list of print jobs queued by the specified user:

`lpstat -u {{user}}`
