# pgbench 
## chatgpt 
The pgbench command is a utility for benchmarking PostgreSQL database systems. It provides a standard set of benchmark tests that can simulate typical database workloads in order to measure the performance and scalability of the system under load.

The pgbench command works by creating a test database and populating it with data using a set of pre-defined scripts. These scripts can be configured to simulate a variety of workloads, including online transaction processing (OLTP) and data warehousing.

Once the test database is set up, the pgbench command runs a series of benchmark tests that simulate database queries and transactions. These tests are designed to stress the system in order to measure its performance and identify any bottlenecks or performance issues.

The output of the pgbench command includes statistics on the number of transactions per second (TPS) and the average latency for each test. This information can be used to compare the performance of different systems or configurations and identify opportunities for optimization.

Overall, the pgbench command is a powerful tool for testing and benchmarking PostgreSQL database systems, and is widely used by developers and administrators to optimize their database performance. 

## tldr 
 
> Run a benchmark test on PostgreSQL.
> More information: <https://www.postgresql.org/docs/10/pgbench.html>.

- Initialize a database with a scale factor of 50 times the default size:

`pgbench --initialize --scale={{50}} {{database_name}}`

- Benchmark a database with 10 clients, 2 worker threads, and 10,000 transactions per client:

`pgbench --client={{10}} --jobs={{2}} --transactions={{10000}} {{database_name}}`
