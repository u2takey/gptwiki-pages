# cronic 
## chatgpt 
Cronic is not a command in the standard Linux or Unix command-line interface. However, it is a Bash shell script command that can be used to run other commands and programs in a way that hides their output unless an error occurs. 

When you run a Bash script using cron (a job scheduler on Unix-like systems), the main problem is that it sends an email to the user containing the output of the script, even if there's no error. This can be problematic if you have a script that runs frequently or that produces a lot of output.

To solve this issue, you can use Cronic, which is designed to capture the output of the scripts it runs and only send an email if an error occurs. The syntax of the command is as follows:

```
cronic [options] command args
```

- [options]: Optional arguments that control the behavior of Cronic. For example, -q suppresses normal output, -p changes the prefix for error messages, and -t sets a timeout for the command.

- command: The command or script to run using Cronic.

- args: Optional arguments to pass to the command.

When you run a command with Cronic, it captures the output (both stdout and stderr) and checks if there's an error (by looking for a non-zero exit status). If there's no error, it silently exits, but if there's an error, it sends an email to the user containing the captured output and the error message.

In summary, Cronic is a Bash script command that can be used to run other commands and scripts in a way that minimizes output and only sends an email to the user if there's an error. 

## tldr 
 
> Bash script for wrapping cron jobs to prevent excess email sending.
> More information: <https://habilis.net/cronic/>.

- Call a command and display its output if it returns a non-zero exit code:

`cronic {{command}}`
