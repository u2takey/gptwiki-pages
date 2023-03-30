# goldeneye.py 
## chatgpt 
GoldenEye.py is a Python script for stress testing web servers. It generates HTTP/HTTPS requests with varying headers and parameters to simulate an attack. The tool was created as a proof-of-concept and is not intended for malicious use. 

When executed, the command invokes the GoldenEye.py script, which can be customized with several options and flags: 

- `-h` or `--help`: displays the help menu 
- `-t` or `--threads`: sets the number of threads used to send requests 
- `-s` or `--sockets`: sets the number of sockets per thread 
- `-r` or `--ramp`: sets the time (in seconds) during which the number of threads will be increased 
- `-g` or `--get`: enables GET requests 
- `-p` or `--post`: enables POST requests 
- `-x` or `--proxy`: enables proxy support 

Below is an example of how to use the command to target a web server with GET requests: 

`python goldeneye.py -t 10 -s 20 -r 10 -g http://example.com`

In this example, the script is set to use 10 threads, each with 20 sockets, and to increase the number of threads over a period of 10 seconds. The `-g` flag is used to indicate that the requests will be GET requests. The target web server is `http://example.com`. 

It is important to note that the use of GoldenEye.py for malicious purposes is illegal and the tool should only be used for authorized testing and research purposes. 

## tldr 
 
> A HTTP DoS test tool.
> More information: <https://github.com/jseidl/GoldenEye>.

- Test a specific website:

`./goldeneye.py {{url}}`

- Test a specific website with 100 user agents and 200 concurrent sockets:

`./goldeneye.py {{url}} --useragents 100 --sockets 200`

- Test a specific website without verifying the SSL certificate:

`./goldeneye.py {{url}} --nosslcheck`

- Test a specific website in debug mode:

`./goldeneye.py {{url}} --debug`

- Display help:

`./goldeneye.py --help`
