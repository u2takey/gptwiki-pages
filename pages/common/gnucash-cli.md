# gnucash-cli 
## chatgpt 
The "gnucash-cli" command is a command line interface to the GnuCash accounting software. It allows users to access and manipulate their GnuCash data files from the command line, without having to open the GnuCash graphical user interface.

The command can be used for a variety of tasks, including importing and exporting data, generating reports, and checking account balances. It can also be used to automate accounting tasks through scripting.

To use the gnucash-cli command, users will need to have GnuCash installed on their system, and they will need to have a GnuCash data file available. They can then open a terminal window and run the gnucash-cli command, followed by any necessary parameters or options.

While powerful, the gnucash-cli command can be complex and may require some knowledge of command line interfaces and accounting principles. Users should consult the GnuCash documentation and seek guidance if they are unsure how to use the command. 

## tldr 
 
> A command-line version of GnuCash.
> More information: <https://gnucash.org>.

- Get quotes for currencies and stocks specified in a file and print them:

`gnucash-cli --quotes get {{path/to/file.gnucash}}`

- Generate a financial report of a specific type, specified by `--name`:

`gnucash-cli --report run --name "{{Balance Sheet}}" {{path/to/file.gnucash}}`
