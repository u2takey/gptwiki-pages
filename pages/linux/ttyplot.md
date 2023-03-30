# ttyplot 
## chatgpt 
The `ttyplot` command is a tool for plotting graphs in the terminal. It is a command-line utility that allows you to plot live or recorded data with minimal setup.

To use `ttyplot`, you need to provide it with data to plot. This can be done in several ways, including reading from a file, piping data from another command, or specifying the data directly on the command line.

Once you have the data, you need to specify how to plot it. `ttyplot` supports a wide variety of plot styles, including line graphs, bar charts, and scatter plots.

You can also customize the plot's appearance by changing the colors, axis labels, grid lines, and other settings.

One of the most useful features of `ttyplot` is its ability to plot data in real-time. You can use it to monitor system performance, network traffic, or other time-based metrics.

Overall, `ttyplot` is a versatile and easy-to-use tool for creating simple but effective visualizations in the terminal. 

## tldr 
 
> A realtime plotting utility for the command line with data input from `stdin`.
> More information: <https://github.com/tenox7/ttyplot>.

- Plot the values `1`, `2` and `3` (`cat` prevents ttyplot to exit):

`{ echo {{1 2 3}}; cat } | ttyplot`

- Set a specific title and unit:

`{ echo {{1 2 3}}; cat } | ttyplot -t {{title}} -u {{unit}}`

- Use a while loop to continuously plot random values:

`{ while {{true}}; do echo {{$RANDOM}}; sleep {{1}}; done } | ttyplot`

- Parse the output from `ping` and visualize it:

`ping {{8.8.8.8}} | sed -u '{{s/^.*time=//g; s/ ms//g}}' | ttyplot -t "{{ping to 8.8.8.8}}" -u {{ms}}`
