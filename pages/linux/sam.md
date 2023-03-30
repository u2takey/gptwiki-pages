# sam 
## chatgpt 
The "sam" command is a utility found in Unix-based operating systems, including Linux and macOS, that is used to manage user accounts on the system. 

The command has several sub-commands that allow you to perform various user account management tasks, including:

1. sam adduser: This command is used to create a new user account on the system. When executed, it opens an interactive shell that prompts you to enter the user's name, password, home directory, group membership, and other account details.

2. sam deleteuser: This command is used to delete a user account from the system. When executed, it prompts you to select the user account you want to delete, and then confirms the deletion before proceeding.

3. sam chuser: This command is used to modify an existing user account. When executed, it opens an interactive shell that allows you to change the user's name, password, home directory, group membership, and other account details.

4. sam listusers: This command is used to display a list of all user accounts on the system. When executed, it prints a table of user account information, including the username, real name, and home directory.

Overall, the "sam" command is a powerful tool for managing user accounts on Unix-based systems, and it can be used to add, delete, and modify user accounts quickly and easily. 

## tldr 
 
> AWS Serverless Application Model (SAM) CLI.
> More information: <https://github.com/awslabs/aws-sam-cli>.

- Initialize a serverless application:

`sam init`

- Initialize a serverless application with a specific runtime:

`sam init --runtime {{python3.7}}`

- Package a SAM application:

`sam package`

- Build your Lambda function code:

`sam build`

- Run your serverless application locally:

`sam local start-api`

- Deploy an AWS SAM application:

`sam deploy`
