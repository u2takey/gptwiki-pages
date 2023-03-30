# parallel 
## chatgpt 
The `parallel` command is a shell utility that allows running shell commands or scripts in parallel. Its purpose is to speed up the execution time of an entire batch of commands by running them simultaneously on multiple processor cores.

The `parallel` command works by splitting the input data into many parts, with each part being passed to a separate instance of the specified command. For example, if the input data is a list of files, each file can be processed by a separate instance of a processing script.

The `parallel` command is highly configurable and supports many complex features. Some of the most commonly used options include:

- `-j N` - Limits the number of jobs run in parallel to N (where N is an integer)
- `-a filename` - Reads the input data from a file instead of standard input
- `-k` - Preserves the order of the output, even when the inputs are processed out of order

Overall, the `parallel` command is a powerful tool for running shell commands in parallel, which can save a considerable amount of time and resources in many cases. 

## tldr 
 
> Run commands on multiple CPU cores.
> More information: <https://www.gnu.org/software/parallel>.

- Gzip several files at once, using all cores:

`parallel gzip ::: {{file1}} {{file2}} {{file3}}`

- Read arguments from `stdin`, run 4 jobs at once:

`ls *.txt | parallel -j4 gzip`

- Convert JPG images to PNG using replacement strings:

`parallel convert {} {.}.png ::: *.jpg`

- Parallel xargs, cram as many args as possible onto one command:

`{{args}} | parallel -X {{command}}`

- Break `stdin` into ~1M blocks, feed each block to `stdin` of new command:

`cat {{big_file.txt}} | parallel --pipe --block 1M {{command}}`

- Run on multiple machines via SSH:

`parallel -S {{machine1}},{{machine2}} {{command}} ::: {{arg1}} {{arg2}}`
