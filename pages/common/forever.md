# forever 
## chatgpt 
The `forever` command is a tool designed to keep Node.js scripts (or any other script or executable) running continuously without the need for manual intervention.

When you run the `forever` command, it starts a daemon process that monitors your script and restarts it if it crashes or terminates for any reason. This ensures that your script runs continuously and is always available to handle incoming requests or perform any other tasks it was designed to perform.

Some common use cases for `forever` include running a server or API that needs to be up and running 24/7 or running a background task that should continue to run even if the user logs out of the system.

To use `forever`, you typically just need to specify the path to your script as an argument. For example, if your script is called `server.js`, you could use the following command to start it with `forever`:

```sh
forever start server.js
```

This will start your script as a background process and keep it running indefinitely. You can then monitor the status of your script using various `forever` commands, such as `forever list` to view all running scripts, `forever stop <id>` to stop a specific script, or `forever stopall` to stop all running scripts.

Overall, the `forever` command is a powerful tool for ensuring that your Node.js scripts (or any other script or executable) run continuously and stay available without the need for manual intervention. 

## tldr 
 
> Server-side JavaScript application that makes sure Node.js applications run indefinitely (restarts after exit).
> More information: <https://github.com/foreversd/forever>.

- Start running a file forever (as a daemon):

`forever {{script}}`

- List running "forever" processes (along with IDs and other details of "forever" processes):

`forever list`

- Stop a running "forever" process:

`forever stop {{ID|pid|script}}`
