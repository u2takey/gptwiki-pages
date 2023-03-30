# speedtest 
## chatgpt 
The "speedtest" command is a network measurement tool used to measure the internet speed of a device. When this command is executed, it sends a signal to the internet service provider (ISP) server and measures the time taken for the server to respond. This response time is used to calculate the download and upload speed of the internet connection.

The speedtest command generally runs a series of tests on the internet connection, including ping, download speed and upload speed test. The ping test measures the time taken for a signal to travel from the device to the server and back. This test helps to determine the quality of the internet connection. The download speed test measures how fast data can be downloaded from the internet to the device, and the upload speed test measures how fast data can be uploaded from the device to the internet.

After completing the tests, the speedtest command will display the download, upload and ping speeds in megabits per second (Mbps) or kilobits per second (Kbps). It may also show additional information, such as the ISP name, server location, and server speed.

Overall, the speedtest command is an efficient way to check the internet connection quality, especially if you are experiencing slow speeds or connectivity issues, and need to troubleshoot the problem. 

## tldr 
 
> Official command-line interface for testing internet bandwidth using https://speedtest.net.
> Note: some platforms link `speedtest` to `speedtest-cli`. If some of the examples in this page don't work, see `speedtest-cli`.
> More information: <https://www.speedtest.net/apps/cli>.

- Run a speed test:

`speedtest`

- Run a speed test and specify the unit of the output:

`speedtest --unit={{auto-decimal-bits|auto-decimal-bytes|auto-binary-bits|auto-binary-bytes}}`

- Run a speed test and specify the output format:

`speedtest --format={{human-readable|csv|tsv|json|jsonl|json-pretty}}`

- Run a speed test and specify the number of decimal points to use (0 to 8, defaults to 2):

`speedtest --precision={{precision}}`

- Run a speed test and print its progress (only available for output format `human-readable` and `json`):

`speedtest --progress={{yes|no}}`

- List all `speedtest.net` servers, sorted by distance:

`speedtest --servers`

- Run a speed test to a specific `speedtest.net` server:

`speedtest --server-id={{server_id}}`
