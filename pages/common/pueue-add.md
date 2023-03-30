# pueue add 
## chatgpt 
The "pueue add" command is used in Pueue, a command-line task manager tool in Unix-like systems, to add a command to a task queue. 

When executed, the command prompts the user for the command to be executed in the future, followed by a set of flags that can be used to configure various settings for the task. These flags include specifying the maximum number of parallel tasks to run, setting priority, defining dependencies, specifying time and date for scheduling, among others. 

Once the user inputs the necessary information, Pueue adds the task to the queue and schedules it for execution according to the specified settings. The task queue is persistently stored in a file, so even if the user closes the terminal or logs out, the tasks remain in the queue and continue to execute once the user logs back in or restarts the system. 

Overall, the "pueue add" command enables users to efficiently manage and automate their workflows by queuing up various commands and setting up dependencies, schedules, and priorities for them. 

## tldr 
 
> Enqueue a task for execution.
> More information: <https://github.com/Nukesor/pueue>.

- Add any command to the default queue:

`pueue add {{command}}`

- Pass a list of flags or arguments to a command when enqueuing:

`pueue add -- {{command --arg -f}}`

- Add a command but do not start it if it's the first in a queue:

`pueue add --stashed -- {{rsync --archive --compress /local/directory /remote/directory}}`

- Add a command to a group and start it immediately, see `pueue group` to manage groups:

`pueue add --immediate --group "{{CPU_intensive}}" -- {{ffmpeg -i input.mp4 frame_%d.png}}`

- Add a command and start it after commands 9 and 12 finish successfully:

`pueue add --after {{9}} {{12}} --group "{{torrents}}" -- {{transmission-cli torrent_file.torrent}}`

- Add a command with a label after some delay has passed, see `pueue enqueue` for valid datetime formats:

`pueue add --label "{{compressing large file}}" --delay "{{wednesday 10:30pm}}" -- "{{7z a compressed_file.7z large_file.xml}}"`
