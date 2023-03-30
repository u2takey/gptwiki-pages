# serverless 
## chatgpt 
"Serverless" is not a command, but a concept or architecture for developing and deploying applications that don't rely on the traditional model of maintaining and managing servers. Instead of running and managing servers, developers can focus on writing code and deploying functions or services that are executed in a serverless environment, which manages the underlying infrastructure and scales automatically based on demand.

In a serverless architecture, developers can use cloud computing services like Amazon Web Services (AWS), Google Cloud Functions, or Microsoft Azure Functions to write and deploy code without worrying about the underlying infrastructure. They pay only for the resources their functions use, such as compute time, memory, and network bandwidth, and are charged on a per-execution basis. This allows developers to focus on building their applications without having to worry about capacity planning, scaling, or infrastructure management.

To implement serverless applications, developers typically use a framework like Serverless Framework or AWS Serverless Application Model (SAM) to define and deploy their functions and services. These frameworks abstract away the underlying infrastructure and provide a declarative way to define functions, APIs, and other resources.

The "serverless" command may refer to a specific tool or framework that enables developers to deploy serverless applications to a cloud computing platform. For example, the "serverless" command in the Serverless Framework can be used to deploy, configure, and manage serverless applications to various cloud computing providers. 

## tldr 
 
> Toolkit for deploying and operating serverless architectures on AWS, Google Cloud, Azure and IBM OpenWhisk.
> Commands can be run either using the `serverless` command or its alias, `sls`.
> More information: <https://serverless.com/>.

- Create a serverless project:

`serverless create`

- Create a serverless project from a template:

`serverless create --template {{template_name}}`

- Deploy to a cloud provider:

`serverless deploy`

- Display information about a serverless project:

`serverless info`

- Invoke a deployed function:

`serverless invoke -f {{function_name}}`

- Follow the logs for a project:

`serverless logs -t`
