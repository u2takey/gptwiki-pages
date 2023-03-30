# sysbench 
## chatgpt 
Sysbench is a multi-platform and multi-threaded benchmarking tool that helps to evaluate and measure the performance of various hardware and software components. It is used to test CPU, memory, file I/O, and database performance on Linux-based systems. Sysbench is available for various Linux distributions, including Ubuntu, Debian, Red Hat, and CentOS.

The sysbench command can be used with various options and sub-commands to perform different types of benchmarks. Here are some examples:

- CPU benchmark: To test the CPU performance of your system, run the following command:

  sysbench cpu run

  This will run a stress test on your CPU by calculating prime numbers up to a specified limit. You can customize the test by specifying the number of threads, time, and CPU mode (single or multi). For example:

  sysbench --num-threads=4 --max-time=10 cpu run

  This will use 4 threads to calculate prime numbers for 10 seconds.

- Memory benchmark: To test the memory performance of your system, run the following command:

  sysbench memory run

  This will allocate a large block of memory and perform read and write operations on it. You can customize the test by specifying the block size, number of threads, and total memory size. For example:

  sysbench --memory-block-size=1M --memory-total-size=10G --num-threads=4 memory run

  This will allocate 10GB of memory and use 4 threads to read and write 1MB blocks.

- File I/O benchmark: To test the file I/O performance of your system, run the following command:

  sysbench fileio prepare

  This will create a set of files to use for the benchmark. You can specify the number of files and their size. For example:

  sysbench --file-total-size=1G --file-test-mode=rndrw --file-block-size=4K fileio prepare

  This will create a 1GB file and set the test mode to read and write randomly with a block size of 4KB.

  Once the files are created, you can run the benchmark using the following command:

  sysbench --file-total-size=1G --file-test-mode=rndrw --file-block-size=4K fileio run

  This will perform read and write operations on the files according to the specified test mode.

- Database benchmark: To test the database performance of your system, you need to install a database server, such as MySQL or PostgreSQL. Sysbench provides a set of benchmarks for these databases, including OLTP (Online Transaction Processing) and read/write tests. Here is an example of an OLTP test for MySQL:

  sysbench oltp_read_write --db-driver=mysql --mysql-host=localhost --mysql-db=test --mysql-user=root --mysql-password=passwd prepare

  This will create a database and a set of tables to use for the test.

  Once the preparation is completed, you can run the benchmark using the following command:

  sysbench oltp_read_write --db-driver=mysql --mysql-host=localhost --mysql-db=test --mysql-user=root --mysql-password=passwd --oltp-tables-count=10 --oltp-table-size=100000 --num-threads=4 run

  This will simulate a workload of 10 tables with 100,000 rows each and use 4 threads to perform read and write operations.

Overall, sysbench is a powerful tool that can help you to identify performance bottlenecks and optimize your system for better performance. 

## tldr 
 
> Benchmark a System's CPU, IO and memory.
> More information: <https://github.com/akopytov/sysbench/>.

- Run a CPU benchmark with 1 thread for 10 seconds:

`sysbench cpu run`

- Run a CPU benchmark with multiple threads for a specified time:

`sysbench --threads={{number_of_threads}} --time={{seconds}}`

- Run a memory benchmark with 1 thread for 10 seconds:

`sysbench memory run`

- Prepare a filesystem-level read benchmark:

`sysbench fileio prepare`

- Run a filesystem-level benchmark:

`sysbench --file-test-mode={{rndrd|rndrw|rndwr|seqrd|seqrewr|seqwr}} fileio run`
