# aws sts 
## chatgpt 
AWS Security Token Service (STS) is a service that enables you to request temporary, limited-privilege credentials for AWS Identity and Access Management (IAM) users or for users that you authenticate (federated users). The AWS STS API Reference describes the low-level STS API operations, which are useful for building more complex and customized STS operations.

The "aws sts" command is used to access the AWS Security Token Service (STS) from the command line interface (CLI). It allows you to view, manage, and assume AWS temporary security credentials.

To use the "aws sts" command, you first need to have the AWS CLI installed and configured with your AWS credentials. Once you have done that, you can use the "aws sts" command to perform various actions, such as:

- "aws sts get-session-token": This command returns a set of temporary security credentials that you can use to authenticate requests to AWS services.

- "aws sts assume-role": This command allows you to assume an IAM role and obtain temporary security credentials that can be used to access resources that require permissions associated with the role.

- "aws sts decode-authorization-message": This command is used to decode the authorization message that you receive when you attempt to access a protected resource.

- "aws sts get-caller-identity": This command returns information about the AWS account to which the credentials belong, as well as the IAM user or role that was used to make the request.

Overall, the "aws sts" command is a powerful tool that enables you to manage security credentials and access to AWS resources from the command line interface. 

## tldr 
 
> Security Token Service (STS) allows to request temporary credentials for (IAM) users or federated users.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/sts/>.

- Get temporary security credentials to access specific AWS resources:

`aws sts assume-role --role-arn {{aws_role_arn}}`

- Get an IAM user or role whose credentials are used to call the operation:

`aws sts get-caller-identity`
