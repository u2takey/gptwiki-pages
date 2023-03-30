# sreport 
## chatgpt 
The command "sreport" is a tool used for reporting information on job and resource usage in a Slurm cluster. It provides various reports in tabular format that can be used to analyze the usage and performance of a cluster.

The usage of the "sreport" command can be broken down into the following syntax:

sreport [global options] [plugin options] [report] [report options]

- Global options: These are the options that apply to all plugins and reports. Examples of global options include "-h" for help, "-u" for specifying a username, and "-n" for specifying the name of the Slurm cluster.
- Plugin options: These are the options that apply to specific plugins or reports. Examples of plugin options include "-t" for specifying a time period, "-P" for specifying a particular partition of the cluster, and "-j" for specifying a specific job or set of jobs.
- Report: This is the specific report that you want to generate. For example, "sreport cluster Utilization" will generate a report on the overall resource utilization of the cluster.
- Report options: These are the options that apply to specific reports. Examples of report options include "-P" for specifying a particular partition, "-t" for specifying a time period, and "-u" for specifying a username.

Overall, the "sreport" command is a powerful tool for monitoring and analyzing the usage and performance of a Slurm cluster. By using various plugins and options, it allows administrators and users to generate detailed reports on a wide range of metrics, from job and resource utilization to billing and charging information. 

## tldr 
 
> Generate reports on jobs, users, and clusters from accounting data.
> More information: <https://slurm.schedmd.com/sreport.html>.

- Show pipe delimited cluster utilization data:

`sreport --parsable cluster utilization`

- Show number of jobs run:

`sreport job sizes printjobcount`

- Show users with the highest CPU time use:

`sreport user topuser`
