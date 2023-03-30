# amixer 
## chatgpt 
The `amixer` command is a command line tool that allows you to control the volume levels of your audio devices in Linux. It is specifically used to interact with ALSA (Advanced Linux Sound Architecture) mixer controls.

Here are some specific options that can be used with `amixer`:

- `scontrols` - Show all available mixer controls
- `scontents` - Show the current value of all mixer controls
- `set <control> <value>` - Set the value of a specific mixer control
- `get <control>` - Get the current value of a specific mixer control
- `mute` - Mute a specific mixer control
- `unmute` - Unmute a specific mixer control

For example, if you want to set the Master volume to 50%, you can use the following command:

```
amixer set Master 50%
```

This will set the Master control to 50% of its maximum volume level. If you want to mute the Master control, you can use the following command:

```
amixer set Master mute
```

This will mute the Master control, and it can be unmuted again by running:

```
amixer set Master unmute
```

Overall, `amixer` is a powerful tool that allows you to fine-tune the audio settings on your Linux system. 

## tldr 
 
> Mixer for ALSA soundcard driver.
> More information: <https://manned.org/amixer>.

- Turn up the master volume by 10%:

`amixer -D pulse sset Master {{10%+}}`

- Turn down the master volume by 10%:

`amixer -D pulse sset Master {{10%-}}`
