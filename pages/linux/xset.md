# xset 
## chatgpt 
The `xset` command is an X Window System utility that allows users to configure various display settings such as screen saver, keyboard, pointer, and font settings for the X server on Linux and Unix-like systems.

Here are some examples of how to use the `xset` command:

1. Changing the screen saver timeout:

The `s` option is used to set the timeout in seconds for the screen saver to activate. To set the timeout to 10 minutes (600 seconds), use the command:

```
xset s 600
```

2. Disabling the screensaver:

To disable the screensaver, use the command:

```
xset s off
```

3. Turning off the screen:

The `dpms` option is used to turn off the screen after a specified amount of time. To turn off the screen after 5 minutes, use the command:

```
xset dpms 300
```

4. Changing the keyboard repeat rate:

The `r` option is used to set the keyboard repeat rate. To set the repeat rate to 30 characters per second, use the command:

```
xset r rate 30
```

Overall, `xset` is a very useful command for customizing various display settings on Linux and Unix-like systems. 

## tldr 
 
> User preference utility for X.
> More information: <https://manned.org/xset>.

- Disable the screensaver:

`xset s off`

- Set the screensaver to start after 60 minutes of inactivity:

`xset s 3600 3600`

- Disable DPMS (Energy Star) features:

`xset -dpms`

- Enable DPMS (Energy Star) features:

`xset +dpms`
