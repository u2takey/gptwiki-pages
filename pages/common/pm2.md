# pm2 
## chatgpt 
pm2 is a process manager for Node.js applications that allows you to monitor, manage, and restart your Node.js processes. Here's a breakdown of some of the most commonly used commands in pm2:

1. pm2 start: Starts your Node.js application as a pm2 process.

2. pm2 stop: Stops a running pm2 process.

3. pm2 restart: Restarts a pm2 process.

4. pm2 delete: Stops and deletes a pm2 process.

5. pm2 list: Lists all pm2 processes that are currently running.

6. pm2 logs: Displays the log output of a pm2 process.

7. pm2 monit: Opens a real-time monitoring dashboard for all pm2 processes.

8. pm2 save: Saves the current list of pm2 processes, so they can be restarted automatically when the system is rebooted.

9. pm2 startup: Generates a startup script to automatically start your pm2 processes when the system boots up. 

Overall, pm2 provides a convenient and reliable way to manage your Node.js processes and keep them running smoothly. 

## tldr 
 
> Process manager for Node.js.
> Used for log management, monitoring and configuring processes.
> More information: <https://pm2.keymetrics.io>.

- Start a process with a name that can be used for later operations:

`pm2 start {{app.js}} --name {{application_name}}`

- List processes:

`pm2 list`

- Monitor all processes:

`pm2 monit`

- Stop a process:

`pm2 stop {{application_name}}`

- Restart a process:

`pm2 restart {{application_name}}`

- Dump all processes for resurrecting them later:

`pm2 save`

- Resurrect previously dumped processes:

`pm2 resurrect`
