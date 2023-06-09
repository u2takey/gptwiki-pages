# http_load 
## chatgpt 
http_load is a performance measurement and load testing tool designed for testing web servers and applications. It is a command-line tool that allows users to simulate multiple concurrent connections to a web server, measure its response time and throughput, and generate a report of the test results.

The http_load command syntax is:

http_load [options] [URL_file]

where [options] are the command-line options and [URL_file] is the name of the file containing a list of URLs to be tested.

Some of the common options used with http_load are:

- "-p" used to set the server port number
- "-t" used to set the maximum time for the test
- "-r" used to set the rate of requests per second
- "-s" used to set the maximum number of connections to be established
- "-n" used to set the number of requests to be made
- "-f" used to set the format of the output report

The [URL_file] contains a list of URLs to be tested, separated by newlines. http_load will randomly select URLs from the list and distribute them evenly among the concurrent connections.

The test results generated by http_load include the number of requests, the total time taken, the average response time, and the throughput. The output report can be saved in various formats like HTML, CSV, or plain text.

In summary, http_load is a powerful tool for load testing web servers and applications, providing useful metrics about their performance and identifying potential performance bottlenecks. 

## tldr 
 
> An HTTP benchmarking tool.
> Runs multiple HTTP fetches in parallel to test the throughput of a web server.
> More information: <http://www.acme.com/software/http_load/>.

- Emulate 20 requests based on a given URL list file per second for 60 seconds:

`http_load -rate {{20}} -seconds {{60}} {{path/to/urls.txt}}`

- Emulate 5 concurrent requests based on a given URL list file for 60 seconds:

`http_load -parallel {{5}} -seconds {{60}} {{path/to/urls.txt}}`

- Emulate 1000 requests at 20 requests per second, based on a given URL list file:

`http_load -rate {{20}} -fetches {{1000}} {{path/to/urls.txt}}`

- Emulate 1000 requests at 5 concurrent requests at a time, based on a given URL list file:

`http_load -parallel {{5}} -fetches {{1000}} {{path/to/urls.txt}}`
