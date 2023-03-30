# nvidia-smi 
## chatgpt 
The "nvidia-smi" command is a command-line tool that allows users to monitor and manage NVIDIA GPU devices on a system. 

When executed, this command presents a table of information about the GPU devices available on the system, such as the GPU ID, name, temperature, memory usage, and processes running on each device. 

This command can also be used to perform certain management tasks on the GPU devices, such as setting the power limit, resetting the device, or profiling the device's performance. 

In summary, "nvidia-smi" is an important tool for managing and monitoring NVIDIA GPU devices, particularly for tasks such as performance tuning, debugging, and system optimization. 

## tldr 
 
> Aid the management and monitoring of NVIDIA GPU devices.
> More information: <https://developer.nvidia.com/nvidia-system-management-interface>.

- Display information on all available GPUs and processes using them:

`nvidia-smi`

- Display more detailed GPU information:

`nvidia-smi --query`

- Monitor overall GPU usage with 1-second update interval:

`nvidia-smi dmon`
