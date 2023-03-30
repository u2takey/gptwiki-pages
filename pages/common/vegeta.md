# vegeta 
## chatgpt 
Vegeta is a command-line tool for running load testing against HTTP APIs and services. It is designed to simulate high volumes of traffic to test the performance and reliability of an API or service. Vegeta allows users to create different types of requests, set headers, and specify how many requests to make per second or in total.

Vegeta can be used to perform different types of tests and measurements such as:

1. Throughput testing - measures how many requests per second an API can handle under different load conditions.

2. Latency testing - measures the response time for each request and calculates the average response time.

3. Error rate testing - measures the number of errors returned by the API under different load conditions.

To use Vegeta, users need to first create a configuration file with the HTTP requests they want to simulate. The configuration file includes details such as URL, headers, and the HTTP method to use (GET, POST, PUT, DELETE).

Once the configuration file is set up, users can run the Vegeta command to initiate the load testing with the specified settings. Vegeta generates a report with the test results, including metrics such as requests per second, average response time, and error rate.

Overall, Vegeta is a powerful tool for load testing and performance tuning of HTTP APIs and services. Its user-friendly interface and powerful features make it a popular choice among developers and system administrators. 

## tldr 
 
> A command-line utility and a library for HTTP load testing.
> See also `ab`.
> More information: <https://github.com/tsenart/vegeta>.

- Launch an attack lasting 30 seconds:

`echo "{{GET https://example.com}}" | vegeta attack -duration={{30s}}`

- Launch an attack on a server with a self-signed HTTPS certificate:

`echo "{{GET https://example.com}}" | vegeta attack -insecure -duration={{30s}}`

- Launch an attack with a rate of 10 requests per second:

`echo "{{GET https://example.com}}" | vegeta attack -duration={{30s}} -rate={{10}}`

- Launch an attack and display a report:

`echo "{{GET https://example.com}}" | vegeta attack -duration={{30s}} | vegeta report`

- Launch an attack and plot the results on a graph (latency over time):

`echo "{{GET https://example.com}}" | vegeta attack -duration={{30s}} | vegeta plot > {{path/to/results.html}}`

- Launch an attack against multiple URLs from a file:

`vegeta attack -duration={{30s}} -targets={{requests.txt}} | vegeta report`
