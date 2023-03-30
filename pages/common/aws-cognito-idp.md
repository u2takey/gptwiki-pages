# aws cognito-idp 
## chatgpt 
AWS Cognito is a user authentication and management service provided by Amazon Web Services (AWS). Cognito has several components that can be accessed via the command line tool called AWS CLI (Command Line Interface). One of these components is Cognito User Pool, which is responsible for user registration, authentication, and authorization. 

The command "aws cognito-idp" refers to the portion of the CLI that deals with the Cognito Identity Provider (IDP). IDP is a component of Cognito User Pool that allows users to authenticate via third-party providers such as Facebook, Google, and Amazon. 

The "aws cognito-idp" command provides a range of subcommands to work with the Cognito IDP. For example, you can create and configure user pools, manage user attributes, create and manage user groups, and so on. 

In summary, the "aws cognito-idp" command is a part of AWS CLI that allows developers to programmatically work with Cognito User Pool's Identity Provider component, providing a convenient way to manage user authentication and authorization in their applications. 

## tldr 
 
> Manage Amazon Cognito user pool and its users and groups using the CLI.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/cognito-idp/index.html>.

- Create a new Cognito user pool:

`aws cognito-idp create-user-pool --pool-name {{name}}`

- List all user pools:

`aws cognito-idp list-user-pools --max-results {{10}}`

- Delete a specific user pool:

`aws cognito-idp delete-user-pool --user-pool-id {{user_pool_id}}`

- Create a user in a specific pool:

`aws cognito-idp admin-create-user --username {{username}} --user-pool-id {{user_pool_id}}`

- List the users of a specific pool:

`aws cognito-idp list-users --user-pool-id {{user_pool_id}}`

- Delete a user from a specific pool:

`aws cognito-idp admin-delete-user --username {{username}} --user-pool-id {{user_pool_id}}`
