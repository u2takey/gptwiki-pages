# lpr 
## chatgpt 
The lpr command is used to send files for printing to a printer connected to the Unix or Linux system. 

Syntax: lpr [options] [filename] 

Options: 
- -P [printer]: Indicates the name of the printer to which the file is to be sent.
- -# [num]: Specifies the number of copies to be printed.
- -C: Prints the file with a class name.
- -J [job]: Prints the file with a job name.
- -U [user]: Print the file with a username.
- -m: Sends an email to the user once the print job is finished.
- -h [host]: Uses a remote printer on the specified host.

Example usage: lpr -P hp-laserjet myfile.txt 

This command will print the file 'myfile.txt' to the printer named 'hp-laserjet'. 

## tldr 
 
> CUPS tool for printing files.
> See also: `lpstat` and `lpadmin`.
> More information: <https://www.cups.org/doc/man-lpr.html>.

- Print a file to the default printer:

`lpr {{path/to/file}}`

- Print 2 copies:

`lpr -# {{2}} {{path/to/file}}`

- Print to a named printer:

`lpr -P {{printer}} {{path/to/file}}`

- Print either a single page (e.g. 2) or a range of pages (e.g. 2–16):

`lpr -o page-ranges={{2|2-16}} {{path/to/file}}`

- Print double-sided either in portrait (long) or in landscape (short):

`lpr -o sides={{two-sided-long-edge|two-sided-short-edge}} {{path/to/file}}`

- Set page size (more options may be available depending on setup):

`lpr -o media={{a4|letter|legal}} {{path/to/file}}`

- Print multiple pages per sheet:

`lpr -o number-up={{2|4|6|9|16}} {{path/to/file}}`
