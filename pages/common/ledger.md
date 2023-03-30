# ledger 
## chatgpt 
The command "ledger" is a powerful accounting tool used in the command line interface (CLI) of Unix-based systems. It is used to create and manage financial accounts of individuals or businesses easily in a systematic and organized way, making it a popular tool among accountants and small business owners.

Below are some of the basic functions of the ledger command:

1. Creating an account: This can be done by using the “ledger -f filename" command. By default, the Ledger command creates a file with the name "ledger.dat" in the current directory, but the file name can be changed using the "-f" option.

2. Adding a transaction: The command "ledger add" followed by the details of the transaction creates a new item in the ledger file. The transaction can be assigned to an account and include other details such as date, description, and amount.

3. Generating reports: The command "ledger balance" is used to generate a report that shows the balance of all accounts in the ledger file. Additionally, there are other report subcommands such as "register," "balance," "print," and "csv" that generate reports in different formats.

4. Performing a search: The command “ledger search” followed by a query keyword lets users search for transactions within the ledger file.

5. Importing data: The command "ledger import" allows importing transactions from other formats, such as CSV or QIF.

Overall, the Ledger command simplifies accounting processes by providing an easy-to-use tool that manages financial accounts efficiently. 

## tldr 
 
> Ledger is a powerful, double-entry accounting system that is accessed from the UNIX command-line.
> More information: <https://www.ledger-cli.org>.

- Print a balance report showing totals:

`ledger balance --file {{path/to/ledger.journal}}`

- List all postings in Expenses ordered by amount:

`ledger register {{expenses}} --sorted {{amount}}`

- Print total Expenses other than Drinks and Food:

`ledger balance {{Expenses}} and not ({{Drinks}} or {{Food}})`

- Print a budget report:

`ledger budget`

- Print summary information about all the postings:

`ledger stats`
