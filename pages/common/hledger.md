# hledger 
## chatgpt 
hledger is a command-line accounting tool that allows users to record financial transactions, generate reports, and manage their budgets. 

When entered into the command line, hledger will bring up a prompt where users can enter various subcommands to perform specific actions. Some common hledger subcommands include:

- `add` - allows users to add new financial transactions to their ledger
- `balance` - displays the current balance of accounts in the ledger
- `register` - displays a register of all transactions in the ledger
- `income` - generates a report of income and expenses for a specified time period

The syntax for using hledger typically involves entering the subcommand followed by any necessary options or arguments. For example, the command `hledger balance` will display the current balance of all accounts in the ledger.

Overall, hledger is a powerful tool for individuals or small businesses who want to manage their finances using the command line. 

## tldr 
 
> A plain text accounting software for the command-line.
> More information: <https://hledger.org>.

- Add transactions to your journal interactively:

`hledger add`

- Show the account hierarchy, using a specific journal file:

`hledger --file {{path/to/file.journal}} accounts --tree`

- Show a monthly income statement:

`hledger incomestatement --monthly --depth 2`

- Print the amount of cash spent on food:

`hledger print assets:cash | hledger -f- -I balance expenses:food --depth 2`
