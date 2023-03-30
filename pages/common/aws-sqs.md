# aws sqs 
## chatgpt 
AWS SQS stands for Amazon Web Services Simple Queue Service. It is a fully managed message queuing service that enables decoupling and scaling of microservices, distributed systems, and serverless applications. The command "aws sqs" is used in the AWS Command Line Interface (CLI) to interact with SQS, and it provides a set of subcommands that allow you to create, manage, and monitor queues, messages, and queue policies. 

The following are some of the subcommands available under "aws sqs":

1. create-queue: This subcommand is used to create a new SQS queue. You can specify the queue name, visibility timeout, maximum message size, and other parameters.

2. list-queues: This subcommand is used to list all the SQS queues in your account. 

3. send-message: This subcommand is used to send a message to an SQS queue. You need to specify the queue URL and the message payload.

4. receive-message: This subcommand is used to retrieve messages from an SQS queue. You need to specify the queue URL and other optional parameters such as visibility timeout and maximum number of messages.

5. delete-message: This subcommand is used to delete a message from an SQS queue. You need to specify the queue URL and the message handle.

6. delete-queue: This subcommand is used to delete an SQS queue. You need to specify the queue URL.

Overall, the "aws sqs" command provides a convenient way to manage your message queues in the cloud, and it can be easily integrated into your automation workflows and scripts. 

## tldr 
 
> Create, delete, and send messages to queues for the AWS SQS service.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/sqs/index.html>.

- List all availables queues:

`aws sqs list-queues`

- Display the URL of a specific queue:

`aws sqs get-queue-url --queue-name {{queue_name}}`

- Create a queue with specific attributes from a file in JSON format:

`aws sqs create-queue --queue-name {{queue_name}} --attributes {{file://path/to/attributes_file.json}}`

- Send a specific message to a queue:

`aws sqs send-message --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}} --message-body "{{message_body}}" --delay-seconds {{delay}} --message-attributes {{file://path/to/attributes_file.json}}`

- Delete the specified message from a queue:

`aws sqs delete-message --queue-url {{https://queue_url}} --receipt-handle {{receipt_handle}}`

- Delete a specific queue:

`aws sqs delete-queue --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}}`

- Delete all messages from the specified queue:

`aws sqs purge-queue --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}}`

- Enable a specific AWS account to send messages to queue:

`aws sqs add-permission --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}} --label {{permission_name}} --aws-account-ids {{account_id}} --actions SendMessage`
