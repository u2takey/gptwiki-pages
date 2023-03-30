# aws lambda 
## chatgpt 
AWS Lambda is a fully-managed, serverless computing service provided by Amazon Web Services (AWS). It allows users to run code without provisioning or managing servers, by simply uploading code and specifying when it should be executed.

The AWS Lambda command line interface (CLI) is a tool that allows developers to manage their Lambda functions from the command line. It provides a set of commands that can be used to create, update, and manage Lambda functions and their associated resources.

Some common commands that can be used with AWS Lambda include:

- create-function: Creates a new Lambda function using the specified configuration settings and code.
- update-function-code: Updates the code associated with an existing Lambda function.
- delete-function: Deletes an existing Lambda function.
- list-functions: Lists all of the Lambda functions associated with the current AWS account.
- invoke: Invokes a specific Lambda function with the specified input data.

Overall, the AWS Lambda command provides a convenient way for developers to manage and deploy their serverless applications and functions, without the need for complex infrastructure configurations or management. 

## tldr 
 
> CLI for AWS lambda.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/lambda/>.

- Run a function:

`aws lambda invoke --function-name {{name}} {{path/to/response}}.json`

- Run a function with an input payload in JSON format:

`aws lambda invoke --function-name {{name}} --payload {{json}} {{path/to/response}}.json`

- List functions:

`aws lambda list-functions`

- Display the configuration of a function:

`aws lambda get-function-configuration --function-name {{name}}`

- List function aliases:

`aws lambda list-aliases --function-name {{name}}`

- Display the reserved concurrency configuration for a function:

`aws lambda get-function-concurrency --function-name {{name}}`

- List which AWS services can invoke the function:

`aws lambda get-policy --function-name {{name}}`
