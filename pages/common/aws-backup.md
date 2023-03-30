# aws backup 
## chatgpt 
The AWS Backup command is a utility that allows users to automate and manage backups of their Amazon Web Services (AWS) resources. AWS Backup simplifies the process of backing up data across AWS services, including EC2 instances, RDS databases, EFS file systems, DynamoDB tables, and others.

The command can be used to create backup plans, backup vaults, and backup selection rules. Backup plans include settings such as frequency, scheduling, retention periods, and backup policies. Backup vaults are the containers where backups are stored, while backup selection rules define the resources that will be backed up.

The AWS Backup command also includes features such as monitoring, reporting, and notifications. It provides users with insight into the status of their backups, including successful and failed backups, and sends notifications when backups are completed or errors occur.

Overall, the AWS Backup command simplifies the management of backups across AWS services, providing users with a centralized and automated solution for protecting their data in the cloud. 

## tldr 
 
> Unified backup service designed to protect Amazon Web Services services and their associated data.
> More information: <https://docs.aws.amazon.com/cli/latest/reference/backup/index.html>.

- Return BackupPlan details for a specific BackupPlanId:

`aws backup get-backup-plan --backup-plan-id {{id}}`

- Create a backup plan using a specific backup plan name and backup rules:

`aws backup create-backup-plan --backup-plan {{plan}}`

- Delete a specific backup plan:

`aws backup delete-backup-plan --backup-plan-id {{id}}`

- Return a list of all active backup plans for the current account:

`aws backup list-backup-plans`

- Display details about your report jobs:

`aws backup list-report-jobs`
