# doctl account 
## chatgpt 
The `doctl account` command is a command used with the DigitalOcean command-line interface tool (Doctl). 

This command retrieves and displays information about the authenticated user's account. When executed, `doctl account` will display the following information:

- Account ID: A unique identifier assigned to the user's DigitalOcean account.
- Email: The email address associated with the account.
- Droplet Limit: The maximum number of Droplets the account can create.
- Floating IP Limit: The maximum number of Floating IPs the account can create.
- Email Verified: Whether or not the email address has been verified.
- UUID: A universally unique identifier assigned to the account.

This command can be helpful when checking the account information or troubleshooting issues related to the account. 

## tldr 
 
> Retrieve information about Digital Ocean accounts.
> More information: <https://docs.digitalocean.com/reference/doctl/reference/account/>.

- Display account info:

`doctl account get`

- Show the hourly API limit, progress towards it, and when the rate limit resets:

`doctl account ratelimit`

- Display help:

`doctl account --help`
