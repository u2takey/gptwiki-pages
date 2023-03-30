# doctl balance 
## chatgpt 
The command "doctl balance" is used with the DigitalOcean command-line interface (CLI), doctl, to view the balance of your DigitalOcean account.

Here is a breakdown of the command and what it does:

1. "doctl" - This is the command required to start any DigitalOcean CLI command. It allows you to interact with your DigitalOcean resources from the terminal.

2. "balance" - This is the specific command that instructs doctl to retrieve the current balance of your DigitalOcean account.

When you run the "doctl balance" command, doctl will retrieve the current balance of your DigitalOcean account and display it in the terminal. This is a useful command to help you keep track of your account spending, especially if you are using DigitalOcean for multiple projects.

It's important to note that you must have a DigitalOcean account and the doctl CLI installed in your system to use this command. Also, you need to have logged in with your DigitalOcean API credentials to access your account information using doctl. 

## tldr 
 
> Show the balance of a Digital Ocean account.
> More information: <https://docs.digitalocean.com/reference/doctl/reference/balance/>.

- Get balance of the account associated with the current context:

`doctl balance get`

- Get the balance of an account associated with an access token:

`doctl balance get --access-token {{access_token}}`

- Get the balance of an account associated with a specified context:

`doctl balance get --context`
