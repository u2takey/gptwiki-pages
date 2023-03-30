# stress 
## chatgpt 
The `stress` command is a tool used to generate CPU and memory workload in a system to simulate high levels of stress. The command is commonly used to test a system's stability or to evaluate its behavior under high load conditions.

The syntax of the `stress` command is as follows:

```
stress [OPTIONS]
```

The options that can be used with the command include:

- `-c`: specifies the number of CPU to use. 
- `-i`: spawns n instances of stress. 
- `-m`: specifies the amount of memory to use.
- `-d`: specifies the number of disk operations. 
- `-t`: sets a time limit for the stress test. 

The default behavior of the command is to stress the CPU for an indefinite period of time. This can be changed by specifying a time limit using the `-t` option.

The `stress` command can be useful in testing the stability and performance of the system or evaluating its behavior under high load conditions. It can also be used for benchmarking purposes to compare the results of different configurations or hardware setups.

Overall, the `stress` command is a powerful tool that can help to identify performance issues and potential system failures under high load conditions. 

## tldr 
 
> A tool to stress test CPU, memory, and IO on a Linux system.
> More information: <https://manned.org/stress>.

- Spawn 4 workers to stress test CPU:

`stress -c {{4}}`

- Spawn 2 workers to stress test IO and timeout after 5 seconds:

`stress -i {{2}} -t {{5}}`

- Spawn 2 workers to stress test memory (each worker allocates 256M bytes):

`stress -m {{2}} --vm-bytes {{256M}}`

- Spawn 2 workers spinning on write()/unlink() (each worker writes 1G bytes):

`stress -d {{2}} --hdd-bytes {{1GB}}`
