# dunstify 
## chatgpt 
dunstify is a command-line tool that sends notification messages to the Dunst Notification Daemon. The command syntax is as follows: 

```
dunstify [OPTIONS] BODY
```

The `BODY` parameter specifies the message body text of the notification.

The available options for the `dunstify` command include:

- `-a, --appname=APPNAME`: Specifies the name of the application generating the notification.
- `-h, --hint=HINT:VALUE`: Sets an optional hint for the notification, which can include things like the notification urgency level, the notification category, the image/icon to display, etc.
- `-i, --icon=ICON`: Specifies the path to an image file to display as the icon for the notification.
- `-r, --replace=ID`: Replaces an existing notification with the same `ID`. This is useful for updating or removing notifications after they have been displayed.
- `-t, --timeout=DURATION`: Sets the display duration for the notification (in ms). The default duration is 5000 ms (5 seconds).
- `-u, --urgency=LEVEL`: Sets the urgency level of the notification (low, normal, critical). This can affect how the notification is displayed, such as the color or sound played.
- `-v, --verbose`: Enables verbose output for debugging purposes.

Overall, `dunstify` is a versatile command for generating customizable notification messages in Linux systems using the Dunst Notification Daemon. 

## tldr 
 
> A notification tool that is an extension of notify-send, but has more features based around dunst.
> Works with all options that work for notify-send.
> More information: <https://github.com/dunst-project/dunst/wiki/Guides>.

- Show a notification with a given title and message:

`dunstify "{{Title}}" "{{Message}}"`

- Show a notification with specified urgency:

`dunstify "{{Title}}" "{{Message}}" -u {{low|normal|critical}}`

- Specify a message ID (overwrites any previous messages with the same ID):

`dunstify "{{Title}}" "{{Message}}" -r {{123}}`

- To see other possible options:

`notify-send --help`
