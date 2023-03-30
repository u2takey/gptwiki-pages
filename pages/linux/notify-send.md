# notify-send 
## chatgpt 
The 'notify-send' command is a Linux command used to send desktop notifications to the user. 

This command sends a notification message to the notification daemon in the user's session. The user will receive a notification message in the form of a popup window, which will appear on their desktop or in the notification area of their panel.

The 'notify-send' command generally takes three parameters:

- The first parameter is the subject or title of the notification.
- The second parameter is the content or message of the notification.
- The third parameter is optional and is used to set the urgency level of the notification. The urgency level can be set to low, normal, or critical.

Here's an example of the command:

notify-send "New Email" "You have received a new email in your inbox" -u critical

In this example, the command will trigger a notification with the title "New Email", message "You have received a new email in your inbox", and urgency level set to critical. 

## tldr 
 
> Uses the current desktop environment's notification system to create a notification.
> More information: <https://manned.org/notify-send>.

- Show a notification with the title "Test" and the content "This is a test":

`notify-send "{{Test}}" "{{This is a test}}"`

- Show a notification with a custom icon:

`notify-send -i {{icon.png}} "{{Test}}" "{{This is a test}}"`

- Show a notification for 5 seconds:

`notify-send -t 5000 "{{Test}}" "{{This is a test}}"`

- Show a notification with an app's icon and name:

`notify-send "{{Test}}" --icon={{google-chrome}} --app-name="{{Google Chrome}}"`
