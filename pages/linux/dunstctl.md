# dunstctl 
## chatgpt 
dunstctl is a command-line interface tool for controlling the dunst daemon. Dunst is a lightweight and customizable notification daemon for Linux with support for desktop notifications, D-Bus, and libnotify.

Here is a breakdown of the dunstctl command:

Syntax: dunstctl [options] [cmd] [args]

Options:
-h, --help: Show help information about the command.
-v, --version: Show version information about the command.

Commands:
history_pop: Remove the last notification history entry.
close: Close the notification with the specified ID.
close-all: Close all notifications.
context: Change the context which the following actions will operate on.
display: Change the display which the following actions will operate on.
set-paused: Pause and unpause the daemon.
set-timeout: Set or get the timeout for the current context.
set-monitored-windows: Set or add or remove the windows to be monitored.
print-paused: Print whether the daemon is currently paused.
print-timeouts: Print timeouts for the current context.
print-history: Print the notification history.
print-contexts: Print the current contexts.
print-count: Print the current number of notifications.

Arguments:
ID: The ID of the notification you want to close.
CONTEXT: The name of the context you want to operate on.
SECONDS: The timeout value for the notifications displayed in the current context.
ACTION: The action you want to perform, such as add, remove, or list.

Overall, dunstctl is a versatile tool that allows users to manage and customize their notification system in Linux. 

## tldr 
 
> Control command for `dunst`.
> More information: <https://manned.org/dunstctl>.

- Pause notifications:

`dunstctl set-paused true`

- Un-pause notifications:

`dunstctl set-paused false`

- Close all notifications:

`dunstctl close-all`

- Display help:

`dunstctl --help`
