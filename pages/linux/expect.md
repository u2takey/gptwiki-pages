# expect 
## chatgpt 
`expect` is a tool used for automating interactive sessions with command-line applications. It is a scripting language that enables you to interact with applications that require user input, such as passwords or login credentials.

The `expect` command allows you to specify what input to send and what output to expect from a program. You can use this to automate repetitive tasks or to interact with command-line applications in a more seamless and efficient manner.

Here's an example of how you might use `expect`:

```
#!/usr/bin/expect

spawn ssh user@server.com

# Wait for the password prompt
expect "password:"

# Send the password
send "password\r"

# Wait for the server prompt
expect ">"

# Send a command
send "ls -la\r"

# Wait for the output
expect ">"

# Print the output
puts $expect_out(buffer)

# Exit
send "exit\r"
expect eof
```

In this example, we're using `expect` to automate an SSH session. We first spawn an SSH connection to a server, then wait for the password prompt. We send the password, wait for the server prompt, and then send an `ls -la` command. We wait for the output, print it to the console, and then exit the session.

Overall, `expect` is a powerful tool for automating interactive command-line applications. It enables you to write scripts that can interact with such applications in a more efficient and streamlined manner. 

## tldr 
 
> Script executor that interacts with other programs that require user input.
> More information: <https://manned.org/expect>.

- Execute an expect script from a file:

`expect {{path/to/file}}`

- Execute a specified expect script:

`expect -c "{{commands}}"`

- Enter an interactive REPL (use `exit` or Ctrl + D to exit):

`expect -i`
