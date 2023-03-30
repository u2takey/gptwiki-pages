# tc 
## chatgpt 
The `tc` command is a Linux utility used to manage traffic control settings on a network interface. It allows administrators and users to configure various network-related parameters such as bandwidth, packet delay, loss, and shaping/queuing policies.

The basic syntax of the `tc` command is:

```
tc [options] [commands] [parameters]
```

Here is a brief explanation of each part of the command:

- `options`: These are various command-line options that modify the behavior of the `tc` command. Some commonly used options include `-s` for displaying statistics, `-r` for resetting statistics, and `-e` for displaying extended information.

- `commands`: The `tc` command supports several subcommands that correspond to different types of traffic control parameters. Some of the commonly used subcommands include `qdisc` (for configuring queuing disciplines), `class` (for defining traffic classes), and `filter` (for filtering packets based on specific attributes).

- `parameters`: These are various options and values used to configure specific traffic control settings. The parameters vary depending on the subcommand being used.

Overall, the `tc` command is a powerful tool that allows Linux system administrators to optimize network performance by controlling various aspects of network traffic. It requires an understanding of network concepts and can be complex to use, but it is essential for users who need to configure advanced networking settings. 

## tldr 
 
> Show / manipulate traffic control settings.
> More information: <https://manned.org/tc>.

- Add constant network delay to outbound packages:

`tc qdisc add dev {{eth0}} root netem delay {{delay_in_milliseconds}}ms`

- Add normal distributed network delay to outbound packages:

`tc qdisc add dev {{eth0}} root netem delay {{mean_delay_ms}}ms {{delay_std_ms}}ms`

- Add package corruption/loss/duplication to a portion of packages:

`tc qdisc add dev {{eth0}} root netem {{corruption|loss|duplication}} {{effect_percentage}}%`

- Limit bandwidth, burst rate and max latency:

`tc qdisc add dev eth0 root tbf rate {{max_bandwith_mb}}mbit burst {{max_burst_rate_kb}}kbit latency {{max_latency_before_drop_ms}}ms`

- Show active traffic control policies:

`tc qdisc show dev {{eth0}}`

- Delete all traffic control rules:

`tc qdisc del dev {{eth0}}`

- Change traffic control rule:

`tc qdisc change dev {{eth0}} root netem {{policy}} {{policy_parameters}}`
