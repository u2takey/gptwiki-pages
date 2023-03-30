# hyperfine 
## chatgpt 
The `hyperfine` command is a benchmarking tool used to measure the execution time of command-line utilities. It can be used to compare the performance of different versions of the same command, or to evaluate the performance of different commands performing similar tasks.

To use `hyperfine`, you simply specify the command(s) to benchmark as arguments, and `hyperfine` will run each command multiple times and report the average execution time, standard deviation, and other statistics.

For example, to benchmark the `ls` command, you would run:

```
$ hyperfine 'ls -l'
```

`hyperfine` would then run `ls -l` multiple times (by default, 10 runs), and report the average execution time and other statistics.

You can also use `hyperfine` to compare multiple commands against each other. For example, to compare the `ls` and `find` commands, you would run:

```
$ hyperfine 'ls -l' 'find .'
```

`hyperfine` would then run each command multiple times and report the average execution time and other statistics for each command.

Overall, `hyperfine` is a useful tool for benchmarking command-line utilities and evaluating their performance. 

## tldr 
 
> A command-line benchmarking tool.
> More information: <https://github.com/sharkdp/hyperfine/>.

- Run a basic benchmark, performing at least 10 runs:

`hyperfine '{{make}}'`

- Run a comparative benchmark:

`hyperfine '{{make target1}}' '{{make target2}}'`

- Change minimum number of benchmarking runs:

`hyperfine --min-runs {{7}} '{{make}}'`

- Perform benchmark with warmup:

`hyperfine --warmup {{5}} '{{make}}'`

- Run a command before each benchmark run (to clear caches, etc.):

`hyperfine --prepare '{{make clean}}' '{{make}}'`

- Run a benchmark where a single parameter changes for each run:

`hyperfine --prepare '{{make clean}}' --parameter-scan {{num_threads}} {{1}} {{10}} '{{make -j {num_threads}}}'`
