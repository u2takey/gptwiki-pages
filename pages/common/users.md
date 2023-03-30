# users 
## chatgpt 
The `users` command displays a list of currently logged-in user names. When the command is executed in a terminal, it will provide a list of user names, each separated by a space.

Here are some key points to understand about the `users` command:

- The `users` command only lists users that are currently logged in. This means that if a user has logged out, they will not appear in the list.
- If multiple users are currently logged in, each user's name will be displayed on a separate line.
- If no users are currently logged in, the `users` command will not display any output.
- The `users` command can be useful for checking who is currently using a system, especially in multi-user environments.
- The `users` command does not require any options or arguments. Simply typing "users" in a terminal will display the list of users.

Overall, the `users` command is a simple but useful tool for quickly checking who is currently logged in to a system. 

## tldr 
 
> Display a list of logged in users.
> See also: `useradd`, `userdel`, `usermod`.
> More information: <https://www.gnu.org/software/coreutils/users>.

- Print logged in usernames:

`users`

- Print logged in usernames according to a given file:

`users {{/var/log/wmtp}}`
