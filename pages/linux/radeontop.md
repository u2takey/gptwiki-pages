# radeontop 
## chatgpt 
radeontop is a command-line utility used to monitor the performance of AMD Radeon graphics processing units (GPUs) in real-time. When executed, the radeontop command launches a terminal-based interface that displays various performance metrics related to the GPU, such as the GPU usage, temperature, clock speed, fan speed, and memory usage.

Here's a brief explanation of some of the key features of the radeontop command:

- GPU usage: This metric represents the percentage of the GPU's processing power that is being used at any given moment. For example, if the GPU usage is 80%, it means that 80% of the GPU's processing power is being utilized by the currently running application or process.

- GPU temperature: This metric represents the temperature of the GPU in degrees Celsius. High temperatures can indicate that the GPU is being overworked, which can lead to performance issues or even hardware damage.

- Clock speed: This metric represents the frequency at which the GPU's clock cycles are running. Higher clock frequencies can lead to better performance, but they can also generate more heat and consume more power.

- Fan speed: This metric represents the speed at which the GPU's cooling fan is spinning. Higher fan speeds can help dissipate heat more efficiently, but they can also generate more noise.

- Memory usage: This metric represents the amount of GPU memory that is being used by the currently running application or process. High memory usage can indicate that the application is demanding a lot of resources from the GPU.

Overall, radeontop is a valuable tool for monitoring and optimizing the performance of AMD Radeon GPUs. By monitoring these key performance metrics in real-time, users can identify any potential bottlenecks or issues with their GPU and take appropriate action to address them. 

## tldr 
 
> Show utilization of AMD GPUs.
> May require root privileges depending on your system.
> More information: <https://github.com/clbr/radeontop>.

- Show the utilization of the default AMD GPU:

`radeontop`

- Enable colored output:

`radeontop --color`

- Select a specific GPU (the bus number is the first number in the output of `lspci`):

`radeontop --bus {{bus_number}}`

- Specify the display refresh rate (higher means more GPU overhead):

`radeontop --ticks {{samples_per_second}}`
