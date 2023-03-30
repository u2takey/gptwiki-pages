# i7z 
## chatgpt 
i7z is a command-line tool that helps monitor Intel Core i7, i5, and i3 CPU performance. It provides detailed information about the current core frequency, temperature, CPU utilization, and power consumption of each core of the processor.

When you run the i7z command, it displays a list of all the CPU cores along with their current state. The tool uses the CPU's MSRs (Model Specific Registers) to gather the data, and then it displays the output in a simple and understandable format.

The information displayed by i7z includes:

- Core frequency: The current operating frequency of each core in MHz. This shows how fast the CPU is running at the moment.
- Temperature: The current temperature of each core in Celsius. This is an important parameter to monitor as high temperatures can damage the CPU.
- Power consumption: The current power consumption of each core in watts. This helps you understand how much power each core is consuming and whether it is performing efficiently.
- C-state residency: The percentage of time each core spent in each C-state (C0 to C6). This helps you understand the energy efficiency of the CPU.

i7z is a useful tool for troubleshooting CPU-related issues, optimizing the performance of your CPU, and monitoring CPU temperatures and power consumption. 

## tldr 
 
> An Intel CPU (only i3, i5 and i7) realtime reporting tool.
> More information: <https://manned.org/i7z>.

- Start i7z (needs to be run in superuser mode):

`sudo i7z`
