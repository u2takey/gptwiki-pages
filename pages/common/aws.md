# aws 
## chatgpt 
"aws" is a command-line interface (CLI) tool provided by Amazon Web Services (AWS) for managing AWS services and resources. This tool provides access to various AWS services and allows users to create, configure, and manage AWS resources through CLI commands.

The "aws" command has numerous subcommands and options that can be used for various purposes. Some of the commonly used subcommands are:

- "configure": This subcommand is used to set up the user's AWS CLI configuration, including access keys, region, and output format.
- "s3": This subcommand is used to access and manage Amazon Simple Storage Service (S3) buckets and objects.
- "ec2": This subcommand is used to manage Amazon Elastic Compute Cloud (EC2) instances and related resources.
- "lambda": This subcommand is used to manage AWS Lambda functions.
- "iam": This subcommand is used to manage AWS Identity and Access Management (IAM) users, groups, policies, and roles.

The "aws" command is a powerful tool for automating AWS management tasks and can be used in shell scripts, batch files, and other automation tools. It also provides a consistent interface across different AWS services and regions, making it easy to work with multiple resources and services. 

## tldr 
 
> The official CLI tool for Amazon Web Services.
> Some subcommands such as `aws s3` have their own usage documentation.
> More information: <https://aws.amazon.com/cli>.

- Configure the AWS Command-line:

`aws configure wizard`

- Configure the AWS Command-line using SSO:

`aws configure sso`

- See help text for the AWS command:

`aws {{command}} help`

- Get the caller identity (used to troubleshoot permissions):

`aws sts get-caller-identity`

- List AWS resources in a region and output in YAML:

`aws dynamodb list-tables --region {{us-east-1}} --output yaml`

- Use auto prompt to help with a command:

`aws iam create-user --cli-auto-prompt`

- Get an interactive wizard for an AWS resource:

`aws dynamodb wizard {{new_table}}`

- Generate a JSON CLI Skeleton (useful for infrastructure as code):

`aws dynamodb update-table --generate-cli-skeleton`
