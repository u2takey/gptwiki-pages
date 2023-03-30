# rtl_sdr 
## chatgpt 
The `rtl_sdr` command is a software-defined radio (SDR) receiver program that uses RTL2832 based DVB-T dongles as an SDR receiver. It is a command-line tool that allows users to receive and process radio signals over a wide frequency range.

The `rtl_sdr` command is typically used in conjunction with other software tools to implement different radio functionalities. For example, it can be used with the `dump1090` tool to capture and decode ADS-B signals from aircraft, allowing users to track flights and monitor air traffic. 

The syntax of the `rtl_sdr` command typically involves specifying a center frequency and a sample rate, as well as any relevant options or modules to be used. The output of the command can be displayed on the terminal or saved to a file for further processing.

Overall, the `rtl_sdr` command is a powerful and versatile tool for radio enthusiasts and professionals alike, providing a flexible way to receive, decode, and analyze radio signals in real-time. 

## tldr 
 
> Raw data recorder for RTL-SDR receivers.
> Data is encoded using I/Q sampling (aka quadrature sampling).
> More information: <https://osmocom.org/projects/rtl-sdr/wiki/Rtl-sdr>.

- Save RAW data from a frequency (specified in Hz) to a file:

`rtl_sdr -f {{100000000}} {{path/to/file}}`

- Pipe data to another program:

`rtl_sdr -f {{100000000}} - | {{aplay}}`

- Read a specified number of samples:

`rtl_sdr -f {{100000000}} -n {{20}} -`

- Specify the sample rate in Hz (ranges 225001-300000 and 900001-3200000):

`rtl_sdr -f {{100000000}} -s {{2400000}} -`

- Specify the device by its index:

`rtl_sdr -f {{100000000}} -d {{0}} -`

- Specify the gain:

`rtl_sdr -f {{100000000}} -g {{20}} -`

- Specify the output block size:

`rtl_sdr -f {{100000000}} -b {{9999999}} -`

- Use synchronous output:

`rtl_sdr -f {{100000000}} -S -`
