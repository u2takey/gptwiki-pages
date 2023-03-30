# speedometer 
## chatgpt 
The "speedometer" command is a terminal-based tool used to get a graphical representation of network traffic utilization in real-time. It shows the amount of data being used and the speed at which it is being sent or received. 

When the "speedometer" command is executed, it displays a real-time graph on the terminal screen that indicates the current network traffic speed. The graph consists of bars that represent the current speed of the incoming and outgoing network traffic, and it is updated dynamically as the amount of network traffic changes.

By default, the speedometer command displays the network traffic in Mbits/s (megabits per second), but it can also be configured to display it in other units such as Kbits/s (kilobits per second) or MB/s (megabytes per second).

Overall, the "speedometer" command is a useful tool for monitoring your network traffic utilization in real-time and can help you identify potential network bottlenecks or issues. 

## tldr 
 
> Python script that shows a network traffic graph in the terminal.
> More information: <http://excess.org/speedometer>.

- Show graph for a specific interface:

`speedometer -r {{eth0}} -t {{eth0}}`
