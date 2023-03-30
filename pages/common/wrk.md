# wrk 
## chatgpt 
The `wrk` command is used to benchmark HTTP services. 

Here is a detailed explanation of the `wrk` command and its options:

**Basic Syntax:** 
```sh
wrk [options] [http[s]://]hostname[:port][/path]
```

**Options:**

- `-c`: Number of connections to keep open (default: 10)

- `-d`: Duration of the test in seconds (default: 10)

- `-t`: Number of threads to use (default: 2)

- `--timeout`: Socket/request timeout in seconds (default: no timeout)

- `--latency`: Print latency statistics (default: false)

- `--rate`: Workrate, in requests per second (default: as fast as possible)

- `--ssl`: Use HTTPS for requests (default: false)

- `--version`: Print version information and exit

**Usage:**

- To perform a benchmark on an HTTP endpoint with default command line settings, run the `wrk` command followed by the URL of the endpoint you want to test:

```sh
wrk http://www.example.com/
```

- To change the number of connections kept open, use the `-c` option:

```sh
wrk -c 100 http://www.example.com/
```

- To change the duration of the test in seconds, use the `-d` option:

```sh
wrk -d 30 http://www.example.com/
```

- To change the number of threads used, use the `-t` option:

```sh
wrk -t 4 http://www.example.com/
```

- To specify a socket/request timeout, use the `--timeout` option:

```sh
wrk --timeout 30 http://www.example.com/
```

- To display latency statistics during the benchmark, use the `--latency` option:

```sh
wrk --latency http://www.example.com/
```

- To specify a workrate, in requests per second, use the `--rate` option:

```sh
wrk --rate 500 http://www.example.com/
```

- To use HTTPS instead of HTTP, use the `--ssl` option:

```sh
wrk --ssl https://www.example.com/
```

- To print the version information and exit, use the `--version` option:

```sh
wrk --version
``` 

## tldr 
 
> HTTP benchmarking tool.
> More information: <https://github.com/wg/wrk>.

- Run a benchmark for `30` seconds, using `12` threads, and keeping `400` HTTP connections open:

`wrk -t{{12}} -c{{400}} -d{{30s}} "{{http://127.0.0.1:8080/index.html}}"`

- Run a benchmark with a custom header:

`wrk -t{{2}} -c{{5}} -d{{5s}} -H "{{Host: example.com}}" "{{http://example.com/index.html}}"`

- Run a benchmark with a request timeout of `2` seconds:

`wrk -t{{2}} -c{{5}} -d{{5s}} --timeout {{2s}} "{{http://example.com/index.html}}"`
