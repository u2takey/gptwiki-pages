# aws ses 
## chatgpt 
AWS SES (Simple Email Service) is a fully managed email service used for sending and receiving emails. It is a powerful tool for managing and sending bulk emails to a large group of recipients. The AWS SES command enables users to interact with the AWS SES service through the command line interface (CLI). 

With the AWS SES command, users can send emails using the Amazon SES SMTP interface or the Amazon SES API. Users can also manage their email reputation by monitoring their bounce rates, complaint rates, and other metrics using the AWS SES command. Additionally, users can configure their email sending domains, set up email forwarding rules, and use email authentication protocols such as DKIM and SPF.

The AWS SES command is part of the AWS CLI tool, which allows for powerful and efficient management of AWS services from the command line. It is a very useful tool for developers and system administrators who want to automate their email workflows and manage their email infrastructure in a programmatic way. 

## tldr 
 
> CLI for AWS Simple Email Service.
> High-scale inbound and outbound cloud email service.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ses/index.html>.

- Create a new receipt rule set:

`aws ses create-receipt-rule-set --rule-set-name {{rule_set_name}} --generate-cli-skeleton`

- Describe the active receipt rule set:

`aws ses describe-active-receipt-rule-set --generate-cli-skeletion`

- Describe a specific receipt rule:

`aws ses describe-receipt-rule --rule-set-name {{rule_set_name}} --rule-name {{rule_name}} --generate-cli-skeleton`

- List all receipt rule sets:

`aws ses list-receipt-rule-sets --starting-token {{token_string}} --max-items {{integer}} --generate-cli-skeleton`

- Delete a specific receipt rule set (the currently active rule set cannot be deleted):

`aws ses delete-receipt-rule-set --rule-set-name {{rule_set_name}} --generate-cli-skeleton`

- Delete a specific receipt rule:

`aws ses delete-receipt-rule --rule-set-name {{rule_set_name}} --rule-name {{rule_name}} --generate-cli-skeleton`

- Send an email:

`aws ses send-email --from {{from_address}} --destination "ToAddresses={{addresses}}" --message "Subject={Data={{subject_text}},Charset=utf8},Body={Text={Data={{body_text}},Charset=utf8},Html={Data={{message_body_containing_html}},Charset=utf8}}"`

- Show help for a specific SES subcommand:

`aws ses {{subcommand}} help`
