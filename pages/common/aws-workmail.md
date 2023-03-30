# aws workmail 
## chatgpt 
The "aws workmail" command is used to interact with the Amazon WorkMail service using the AWS Command Line Interface (CLI).

Amazon WorkMail is a secure, managed business email and calendaring service that supports existing desktop and mobile email clients. With Amazon WorkMail, users can access their email, contacts, and calendars using Microsoft Outlook, webmail, or their native iOS and Android email applications. The service integrates with other AWS services such as Amazon S3 for storage and retrieval of email content, Amazon CloudTrail for logging, and Amazon SNS for notifications.

Using the "aws workmail" command, users can perform operations such as creating and managing WorkMail organizations, managing WorkMail users and their mailboxes, setting up email rules, configuring email forwarding, and accessing WorkMail data using APIs.

Some of the common "aws workmail" subcommands include:

- workmail create-organization: Create a new Amazon WorkMail organization
- workmail delete-organization: Delete an existing Amazon WorkMail organization
- workmail create-user: Create a new user in a specified Amazon WorkMail organization
- workmail delete-user: Delete an existing user from an Amazon WorkMail organization
- workmail reset-password: Reset the password for a given user in an Amazon WorkMail organization. 

## tldr 
 
> Manage Amazon WorkMail using the CLI.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/workmail/index.html>.

- List all WorkMail organizations:

`aws workmail list-organizations`

- List all users of a specific organization:

`aws workmail list-users --organization-id {{organization_id}}`

- Create a WorkMail user in a specific organization:

`aws workmail create-user --name {{username}} --display-name {{name}} --password {{password}} --organization-id {{organization_id}}`

- Register and enable a group/user to WorkMail:

`aws workmail register-to-work-mail --entity-id {{entity_id}} --email {{email}} --organization-id {{organization_id}}`

- Create a WorkMail group in a specific organization:

`aws workmail create-group --name {{group_name}} --organization-id {{organization_id}}`

- Associate a member to a specific group:

`aws workmail associate-member-to-group --group-id {{group_id}} --member-id {{member_id}} --organization-id {{organization_id}}`

- Deregister and disable a user/group from WorkMail:

`aws workmail deregister-from-work-mail --entity-id {{entity_id}} --organization-id {{organization_id}}`

- Delete a user from an organization:

`aws workmail delete-user --user-id {{user_id}} --organization-id {{organization_id}}`
