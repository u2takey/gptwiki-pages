# salt-run 
## chatgpt 
`salt-run` is a command in the SaltStack framework that runs one or more Salt runners. Salt runners are modules used to execute certain operations or tasks that don't fit into Salt's normal Salt state format.

When executed, the `salt-run` command will search for available runners in the Salt file system and execute the ones specified on the command line. Runners are not tied to any particular minion or target and can be executed from the Salt master or any minion.

Here are some examples of `salt-run` commands:

- `salt-run manage.up`: This will return a list of Salt minions that are currently up and available for communication.
- `salt-run fileserver.update`: This will update the Salt fileserver with any new files placed in the appropriate directories.
- `salt-run jobs.list_jobs`: This will return a list of all Salt jobs currently running on the Salt master or minion.

Overall, `salt-run` is a powerful command that allows you to execute complex operations and tasks that wouldn't otherwise be possible within the Salt state format. 

## tldr 
 
> Frontend for executing salt-runners on minions.
> More information: <https://docs.saltstack.com/ref/cli/salt-run.html>.

- Show status of all minions:

`salt-run manage.status`

- Show all minions which are disconnected:

`salt-run manage.up`
