# aws-google-auth 
## chatgpt 
As an AI language model, my training data only goes until early 2021, and I am not aware of any specific "aws-google-auth" command in use at that time. However, I can still explain what this command might be based on general knowledge of the AWS and Google Cloud platforms.

The "aws-google-auth" command could potentially refer to a tool or script that provides authentication and authorization integration between the AWS and Google Cloud platforms. This tool might work by generating temporary AWS credentials for a user authenticated through their Google Cloud account.

One possible use case for this type of command would be for developers or DevOps engineers who need to interact with both AWS and Google Cloud resources, but want to avoid having to switch between different credential sets or maintain separate login sessions for each platform.

In general, tools like this would be configured with certain parameters, such as the user's Google Cloud account information, the AWS role permissions they need, and any required environment variables or API keys. Users would then run the command to authenticate and obtain temporary AWS credentials based on their Google Cloud login.

Overall, the "aws-google-auth" command would be an example of a useful integration tool for cloud computing environments, helping users save time and streamline their workflows. 

## tldr 
 
> Command-line tool to acquire AWS temporary (STS) credentials using Google Apps as a federated (Single Sign-On) provider.
> More information: <https://github.com/cevoaustralia/aws-google-auth>.

- Log in with Google SSO using the IDP and SP identifiers and set the credentials duration to one hour:

`aws-google-auth -u {{example@example.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}}`

- Log in [a]sking which role to use (in case of several available SAML roles):

`aws-google-auth -u {{example@example.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}} -a`

- Resolve aliases for AWS accounts:

`aws-google-auth -u {{example@example.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}} -a --resolve-aliases`

- Show help information:

`aws-google-auth -h`
