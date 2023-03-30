# httping 
## chatgpt 
httping is a command-line tool that sends HTTP requests to a web server and measures the time it takes for the server to respond. It is similar to the popular ping command, but instead of sending ICMP packets for network testing, httping uses HTTP requests to test the responsiveness of a web server. 

The httping command has several options that can be used to customize the request and measure the response time. Some of the key options are:

- -c: Specifies the number of requests to send. By default, httping sends a single request.
- -t: Specifies the timeout for each request in milliseconds. If the server does not respond within this time, the request is considered failed.
- -i: Specifies the interval between requests in milliseconds. By default, httping sends requests as quickly as possible.
- -p: Specifies the TCP port to use for the request. By default, httping uses port 80 for HTTP requests.
- -s: Specifies the size of the HTTP request data in bytes. By default, httping sends an empty request.
- -m: Specifies the HTTP request method to use, such as GET, POST, or HEAD. By default, httping uses the GET method.
- -v: Enables verbose output, showing details of the request and response.

After sending the requests, httping displays a summary of the results, including the number of successful requests, the average response time, and the standard deviation of the response times. It can also output the raw response data for each request. 

Overall, httping is a useful tool for testing the responsiveness of a web server and diagnosing network or server performance issues. 

## tldr 
 
> Measure the latency and throughput of a web server.
> More information: <https://manned.org/httping>.

- Ping the specified URL:

`httping -g {{url}}`

- Ping the web server on `host` and `port`:

`httping -h {{host}} -p {{port}}`

- Ping the web server on `host` using a TLS connection:

`httping -l -g https://{{host}}`

- Ping the web server on `host` using HTTP basic authentication:

`httping -g http://{{host}} -U {{username}} -P {{password}}`
