# scriptreplay 
## chatgpt 
The command 'scriptreplay' is used to replay the timing and typescript of a terminal session that has been recorded using the 'script' command. The command takes two input files, the first being the output of the 'script' command (typescript), which contains all the input and output of the original terminal session, and the second file being a timing file, which contains the timing information for the input and output of the original session.

The command replays the terminal session in a manner that is similar to the original session, but the timing and speed of the replay can be controlled using the second input file. The command can be used to recreate a session that was previously recorded, or to simulate a session for testing or training purposes.

The 'scriptreplay' command has several options that can be used to control the replay of the session, such as the ability to set the replay speed, delay the start of the replay, or merge multiple sessions together.

Syntax: 

    scriptreplay [options] timingfile [typescript [divisor]]

Options:

    -t, --maxdelay <time>    : set maximum time delay between packets
    -s, --speed <speed>      : set speed of replay
    -d, --divisor <divisor>  : set divisor for timings
    -m, --merge              : merge input files into one session
    -v, --version            : display version information and exit
    -h, --help               : display help message and exit

Example:

To replay a session that was previously recorded using the 'script' command, you can use the following command:

    scriptreplay timingfile typescript

Here, 'timingfile' is the timing file for the session and 'typescript' is the typescript file that contains the input and output of the session. 

You can also specify a replay speed by using the '-s' option, as follows:

    scriptreplay -s 2 timingfile typescript

This command will replay the session at twice the speed of the original session. Additionally, if there are multiple sessions that need to be merged into a single session, you can use the '-m' option, as follows:

    scriptreplay -m timingfile1:typescript1 timingfile2:typescript2

This command will merge two sessions recorded in 'timingfile1' and 'timingfile2', and replay them as a single session. 

## tldr 
 
> Replay a typescript created by the `script` command to the standard output.
> More information: <https://manned.org/scriptreplay>.

- Replay a typescript at the speed it was recorded:

`scriptreplay {{path/to/timing_file}} {{path/to/typescript}}`

- Replay a typescript at double the original speed:

`scriptreplay {{path/to/timingfile}} {{path/to/typescript}} 2`

- Replay a typescript at half the original speed:

`scriptreplay {{path/to/timingfile}} {{path/to/typescript}} 0.5`
