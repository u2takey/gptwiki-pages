# lscpu 
## chatgpt 
The command "lscpu" is a Linux command that is used to display the CPU architecture information, model name, clock speed, cache size and other CPU-related details on the system running the command. The output of the command may vary depending on the system configuration but typically would include details such as:

- Architecture: This will indicate whether the system is using a 32-bit or 64-bit architecture
- CPU op-mode(s): This will indicate which processing modes are available, such as 32-bit, 64-bit, or both
- Byte Order: This will indicate whether the system is using a little or big endian byte order
- CPU(s): This will indicate the number of CPUs or processing cores available on the system
- On-line CPU(s) list: This will indicate the list of CPUs that are presently online
- Thread(s) per core: This will indicate the number of threads that can run on each processing core
- Core(s) per socket: This will indicate the number of processing cores present on each CPU socket
- Socket(s): This will indicate the number of sockets or physical CPUs present on the system
- NUMA node(s): This will indicate the number of Non-Uniform Memory Access nodes present on the system
- Vendor ID: This will indicate the CPU model and vendor
- CPU family, model, and stepping: This will indicate the architecture and model of the CPU
- CPU MHz: This will indicate the clock speed of the CPU
- BogoMIPS: This will indicate a rough estimate of CPU speed in Million Instructions Per Second (MIPS)
- L1d cache, L1i cache, L2 cache, L3 cache: This will indicate the cache sizes for various levels of cache present on the CPU

Overall, the "lscpu" command provides a quick and easy way to gather CPU architecture information and understand the processing capabilities of the system. 

## tldr 
 
> Displays information about the CPU architecture.
> More information: <https://manned.org/lscpu>.

- Display information about all CPUs:

`lscpu`

- Display information in a table:

`lscpu --extended`

- Display only information about offline CPUs in a table:

`lscpu --extended --offline`
