# prosodyctl 
## chatgpt 
Prosodyctl is a command-line utility tool used for managing and controlling the Prosody XMPP server. Prosody is an open-source XMPP (Extensible Messaging and Presence Protocol) communication platform that enables real-time instant messaging, voice and video communication, file sharing, and more.

The prosodyctl command is used for various administrative tasks such as:

1. Creating and managing user accounts
2. Creating and managing virtual hosts
3. Viewing server status and logs
4. Creating and managing SSL certificates
5. Editing configuration files
6. Restarting, stopping, and starting the Prosody server

To use prosodyctl, you first need to navigate (cd) to the directory where the file is stored (typically /usr/bin/prosodyctl) and use it with the appropriate command-line options. For example, to view the status of the Prosody server, you can use the following command:

```
prosodyctl status
```

This command will display information about the server such as uptime, number of connected clients, and memory usage.

Similarly, to create a new user account, you can use the following command:

```
prosodyctl adduser username@yourdomain.com
```

This command will prompt you to enter a password and confirm it. Once you have done that, the new account will be created.

In summary, prosodyctl is a powerful command-line tool that enables you to manage and control the Prosody XMPP server. It is an essential component of the Prosody server that enables you to create and manage user accounts, virtual hosts, SSL certificates, and more. 

## tldr 
 
> The control tool for the Prosody XMPP server.
> More information: <https://prosody.im/doc/prosodyctl>.

- Show the status of the Prosody server:

`sudo prosodyctl status`

- Reload the server's configuration files:

`sudo prosodyctl reload`

- Add a user to the Prosody XMPP server:

`sudo prosodyctl adduser {{user@example.com}}`

- Set a user's password:

`sudo prosodyctl passwd {{user@example.com}}`

- Permanently delete a user:

`sudo prosodyctl deluser {{user@example.com}}`
