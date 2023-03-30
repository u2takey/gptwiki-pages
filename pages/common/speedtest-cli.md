# speedtest-cli 
## chatgpt 
The command "speedtest-cli" is a command-line interface tool used to test the speed of the internet connection. When executed, this tool checks the current download and upload speeds of the internet connection by connecting to a nearby server. It is developed using Python programming language, and it can be installed on Linux, Windows, and macOS operating systems.

The speedtest-cli tool works by using the Python library "speedtest.net" which connects to a server and measures the upload and download speeds. It uses the command-line interface so that the user can execute it easily without the need for a graphical interface.

The speedtest-cli tool provides information such as the download and upload speeds, latency, and the name of the internet service provider. This information helps users to know if their internet connection is slow or fast and can be useful in determining if there are issues with their network connectivity. 

Overall, the "speedtest-cli" command is a useful tool for both professionals and individuals who want to measure the speed of their internet connection with ease. 

## tldr 
 
> Unofficial command-line interface for testing internet bandwidth using https://speedtest.net.
> See also `speedtest` for the official CLI.
> More information: <https://github.com/sivel/speedtest-cli>.

- Run a speed test:

`speedtest-cli`

- Run a speed test and display values in bytes, instead of bits:

`speedtest-cli --bytes`

- Run a speed test using `HTTPS`, instead of `HTTP`:

`speedtest-cli --secure`

- Run a speed test without performing download tests:

`speedtest-cli --no-download`

- Run a speed test and generate an image of the results:

`speedtest-cli --share`

- List all `speedtest.net` servers, sorted by distance:

`speedtest-cli --list`

- Run a speed test to a specific speedtest.net server:

`speedtest-cli --server {{server_id}}`

- Run a speed test and display the results as JSON (suppresses progress information):

`speedtest-cli --json`
