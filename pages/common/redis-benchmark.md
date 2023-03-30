# redis-benchmark 
## chatgpt 
Redis-benchmark is a command-line tool used to benchmark the performance of a Redis server by simulating different client workloads. It can be used to test and optimize various aspects of a Redis deployment, including:

1. Redis throughput: It measures the number of Redis commands processed per second.

2. Redis latency: It measures the time taken by Redis to process each command.

3. Redis memory usage: It measures the amount of memory used by Redis for storing data.

4. Redis CPU usage: It measures the amount of CPU time used by Redis for processing commands.

The redis-benchmark command takes several arguments, including:

1. -h : The hostname or IP address of the Redis server.

2. -p : The port number on which Redis is listening.

3. -c : The number of clients to simulate.

4. -n : The total number of requests to send.

5. -t : The type of test to run, such as set, get, or ping.

6. -k : Whether to generate random keys.

7. -d : The size of the data to send in bytes.

The output of the redis-benchmark command includes several performance metrics, such as the total number of requests processed, the average throughput, the average latency, and the percentage of CPU usage. This information can be used to identify bottlenecks in a Redis deployment and optimize its performance. 

## tldr 
 
> A tool to benchmark a Redis server.
> More information: <https://redis.io/docs/reference/optimization/benchmarks/>.

- Run full benchmark:

`redis-benchmark`

- Run benchmark on a specific Redis server:

`redis-benchmark -h {{host}} -p {{port}} -a {{password}}`

- Run a subset of tests with default 100000 requests:

`redis-benchmark -h {{host}} -p {{port}} -t {{set,lpush}} -n {{100000}}`

- Run with a specific script:

`redis-benchmark -n {{100000}} script load "{{redis.call('set', 'foo', 'bar')}}"`

- Run benchmark by using 100000 [r]andom keys:

`redis-benchmark -t {{set}} -r {{100000}}`

- Run benchmark by using a [P]ipelining of 16 commands:

`redis-benchmark -n {{1000000}} -t {{set,get}} -P {{16}}`

- Run benchmark [q]uietly and only show query per seconds result:

`redis-benchmark -q`
