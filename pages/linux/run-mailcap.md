# run-mailcap 
## chatgpt 
The "run-mailcap" command is a utility that runs the appropriate program to view or process the content of a specified file based on its MIME type. MIME (Multipurpose Internet Mail Extensions) is a standard that defines the nature and format of files within the Internet.

When you run the "run-mailcap" command, it reads a configuration file called "mailcap" that contains a list of MIME types and the corresponding programs or commands to handle them. The command then determines the MIME type of the specified file and executes the program or command associated with that MIME type.

For example, if you have a PDF file and you run the "run-mailcap" command on it, the command will check the "mailcap" configuration file for the MIME type of the PDF file, which is "application/pdf". It will then execute the appropriate PDF viewer to open the file. If there are multiple programs or commands defined for the same MIME type, "run-mailcap" will display a menu asking you to choose which program to use.

In summary, the "run-mailcap" command is a useful utility for automatically opening and processing files based on their MIME types, without needing to know the specific program or command required to handle each file type. 

## tldr 
 
> Run MailCap Programs.
> Run mailcap view, see, edit, compose, print - execute programs via entries in the mailcap file (or any of its aliases) will use the given action to process each mime-type/file.
> More information: <https://manned.org/run-mailcap>.

- Individual actions/programs on run-mailcap can be invoked with action flag:

`run-mailcap --action=ACTION [--option[=value]]`

- In simple language:

`run-mailcap --action=ACTION {{filename}}`

- Turn on extra information:

`run-mailcap --action=ACTION --debug {{filename}}`

- Ignore any "copiousoutput" directive and forward output to standard output:

`run-mailcap --action=ACTION --nopager {{filename}}`

- Display the found command without actually executing it:

`run-mailcap --action=ACTION --norun {{filename}}`
