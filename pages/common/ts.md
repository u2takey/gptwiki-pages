# ts 
## chatgpt 
The "ts" command is used to prepend timestamps to the output of another command. 

Syntax: `ts [options] command`

Options:
- `-s` or `--seconds`: Displays the timestamp in seconds since the epoch (default).
- `-i` or `--iso`: Displays the timestamp in ISO-8601 format.
- `-I` or `--iso-strict`: Displays the timestamp in strict ISO-8601 format.
- `-r` or `--reference`: Uses the timestamp of a reference file instead of the current time.
- `-d` or `--date`: Uses a specific date/time instead of the current time.
- `-h` or `--help`: Displays the help message.

Example: `ts date`

In the above example, the "date" command will be executed and the output will be prepended with a timestamp showing the current date and time in seconds since the epoch. 

Output: `1610811206 Fri Jan 15 09:13:26 UTC 2021`

This command can be useful for troubleshooting, logging, and debugging purposes. 

## tldr 
 
> Add timestamps to every line from standard input.
> More information: <https://joeyh.name/code/moreutils/>.

- Add a timestamp to the beginning of each line:

`{{some_command}} | ts`

- Add timestamps with microsecond precision:

`{{some_command}} | ts "{{%b %d %H:%M:%.S}}"`

- Add [i]ncremental timestamps with microsecond precision, starting from zero:

`{{some_command}} | ts -i "{{%H:%M:%.S}}"`

- Convert existing timestamps in a text file (eg. a log file) into [r]elative format:

`cat {{path/to/file}} | ts -r`
