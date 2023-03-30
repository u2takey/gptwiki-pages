# aws quicksight 
## chatgpt 
"aws quicksight" is a command-line interface (CLI) provided by Amazon Web Services (AWS) for Amazon QuickSight service. 

Amazon QuickSight is a cloud-based business intelligence (BI) service that helps users to analyze data and create interactive visualizations and dashboards. The aws quicksight command can be used to perform various tasks related to QuickSight service such as creating and managing data sources, creating and publishing dashboards, managing user access and permissions, and more.

Here are some examples of the aws quicksight command:

1. To create a new QuickSight data source, you can use the following command:

aws quicksight create-data-source --cli-input-json file://datasource.json

The "datasource.json" file contains the configuration details for the new data source, including the data source type, connection details, and other metadata.

2. To create a new QuickSight dashboard:

aws quicksight create-dashboard --cli-input-json file://dashboard.json

The "dashboard.json" file contains the configuration details for the new dashboard, including the visualization widgets, the data source, and other metadata.

3. To manage user access and permissions:

aws quicksight create-user --aws-account-id 123456789012 --namespace default --identity-type IAM --user-role READER --session-name "session1" 

This command creates a new QuickSight user and assigns them the "READER" role, allowing them to view and interact with dashboards. The "session-name" option creates a temporary session for the user, which can be useful for providing temporary access to external users.

In summary, the aws quicksight command provides a powerful and flexible way to manage and interact with QuickSight service using the command line. It can be a very useful tool for automating QuickSight tasks, performing bulk operations, and integrating QuickSight with other AWS services. 

## tldr 
 
> CLI for AWS QuickSight.
> Access QuickSight entities.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/quicksight/>.

- List datasets:

`aws quicksight list-data-sets --aws-account-id {{aws_account_id}}`

- List users:

`aws quicksight list-users --aws-account-id {{aws_account_id}} --namespace default`

- List groups:

`aws quicksight list-groups --aws-account-id {{aws_account_id}} --namespace default`

- List dashboards:

`aws quicksight list-dashboards --aws-account-id {{aws_account_id}}`

- Display detailed information about a dataset:

`aws quicksight describe-data-set --aws-account-id {{aws_account_id}} --data-set-id {{data_set_id}}`

- Display who has access to the dataset and what kind of actions they can perform on the dataset:

`aws quicksight describe-data-set-permissions --aws-account-id {{aws_account_id}} --data-set-id {{data_set_id}}`
