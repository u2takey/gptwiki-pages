# noti 
## chatgpt 
As an AI language model, I am not sure which "noti" command you are referring to. Can you please provide more context or information about the command, such as the operating system and any additional parameters that may be associated with it? 

## tldr 
 
> Monitor a process and trigger a banner notification.
> More information: <https://github.com/variadico/noti>.

- Display a notification when tar finishes compressing files:

`noti {{tar -cjf example.tar.bz2 example/}}`

- Display a notification even when you put it after the command to watch:

`{{command_to_watch}}; noti`

- Monitor a process by PID and trigger a notification when the PID disappears:

`noti -w {{process_id}}`
