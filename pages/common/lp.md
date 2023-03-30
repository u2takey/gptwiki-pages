# lp 
## chatgpt 
The "lp" command is a basic Linux command used to print files on a printer. Its syntax is typically as follows:

lp [options] [file]

Here are some of the commonly used options for the "lp" command:

- "-d printer": Specify the name of the printer to use.
- "-n num-copies": Specify the number of copies to print.
- "-o optionname=value": Set a specific option for the printer, such as page orientation or paper size.
- "-q priority": Set the print job's priority level.

Here is an example usage of the "lp" command:

lp -d myprinter document.txt

This command will print the "document.txt" file on the printer named "myprinter". It will use the default options for the printer, such as paper size and orientation. If you want to specify additional options, you can use the "-o" option followed by the name of the option and its value. For example:

lp -d myprinter -o page-left=72 -o page-right=72 document.txt

This command will print the "document.txt" file on the "myprinter" printer, with a left margin of 72 units and a right margin of 72 units. 

## tldr 
 
> Print files.
> More information: <https://manned.org/lp>.

- Print the output of a command to the default printer (see `lpstat` command):

`echo "test" | lp`

- Print a file to the default printer:

`lp {{path/to/filename}}`

- Print a file to a named printer (see `lpstat` command):

`lp -d {{printer_name}} {{path/to/filename}}`

- Print N copies of file to default printer (replace N with desired number of copies):

`lp -n {{N}} {{path/to/filename}}`

- Print only certain pages to the default printer (print pages 1, 3-5, and 16):

`lp -P 1,3-5,16 {{path/to/filename}}`

- Resume printing a job:

`lp -i {{job_id}} -H resume`
