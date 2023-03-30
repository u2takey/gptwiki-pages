# aws secretsmanager 
## chatgpt 
AWS Secrets Manager is a fully managed secrets management service that enables you to store, retrieve, and manage secrets such as database credentials, passwords, and API keys throughout their lifecycle.

When you run the command "aws secretsmanager" in the AWS Command Line Interface (CLI), it allows you to manage the Secrets Manager service and perform various actions on secrets. 

Some of the actions that can be performed include:
- Create a new secret
- Update an existing secret
- Retrieve the value of a secret
- Configure rotation policy for a secret
- Delete a secret

The Secrets Manager service uses a pay-as-you-go pricing model, which means you only pay for what you use, and pricing is based on the number of secrets stored and requests made. The Secrets Manager also integrates with other AWS services and provides a secure and scalable solution for managing secrets in the cloud. 

## tldr 
 
> Store, manage, and retrieve secrets.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/secretsmanager/>.

- Show secrets stored by the secrets manager in the current account:

`aws secretsmanager list-secrets`

- Create a secret:

`aws secretsmanager create-secret --name {{name}} --description "{{secret_description}}" --secret-string {{secret}}`

- Delete a secret:

`aws secretsmanager delete-secret --secret-id {{name_or_arn}}`

- View details of a secret except for secret text:

`aws secretsmanager describe-secret --secret-id {{name_or_arn}}`

- Retrieve the value of a secret (to get the latest version of the secret omit `--version-stage`):

`aws secretsmanager get-secret-value --secret-id {{name_or_arn}} --version-stage {{version_of_secret}}`

- Rotate the secret immediately using a Lambda function:

`aws secretsmanager rotate-secret --secret-id {{name_or_arn}} --rotation-lambda-arn {{arn_of_lambda_function}}`

- Rotate the secret automatically every 30 days using a Lambda function:

`aws secretsmanager rotate-secret --secret-id {{name_or_arn}} --rotation-lambda-arn {{arn_of_lambda_function}} --rotation-rules AutomaticallyAfterDays={{30}}`
