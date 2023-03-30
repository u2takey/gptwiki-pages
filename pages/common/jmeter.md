# jmeter 
## chatgpt 
JMeter is an open-source software testing tool developed by the Apache Software Foundation. It is primarily used for load testing, performance testing, and functional testing of websites and web applications.

When the command "jmeter" is executed, it launches the JMeter GUI (Graphical User Interface) interface, which allows users to create and execute test plans. This interface provides users with a set of tools and features necessary to create and run test scripts.

Once the GUI interface is open, users can create a new test plan or open an existing one. A test plan consists of one or more thread groups, which contain one or more samplers (requests) and one or more assertions (checks).

The samplers represent the requests sent to the server under test, and the assertions are used to validate the response received from the server. Users can also add pre-processors, post-processors, and timers to the test plan to simulate different scenarios.

After creating a test plan, users can run it by clicking the "Run" button. JMeter then generates a report showing the results of the test. The report includes information such as response times, throughput, and error rates.

Overall, the "jmeter" command is a powerful tool for software testing and can help software developers and testers identify and fix issues before releasing their software to the public. 

## tldr 
 
> Open source java application designed for load testing functional behavior and measure performance.
> More information: <https://jmeter.apache.org>.

- Run a specific test plan in nongui mode:

`jmeter --nongui --testfile {{path/to/file}}.jmx`

- Run a test plan in nongui mode using a specific log file:

`jmeter --nogui --testfile {{path/to/file}}.jmx --logfile {{path/to/logfile}}.jtl`

- Run a test plan in nongui mode using a specific proxy:

`jmeter --nongui --testfile {{path/to/file}}.jmx --proxyHost {{127.0.0.1}} --proxyPort {{8888}}`

- Run a test plan in nongui mode using a specific JMeter property:

`jmeter --jmeterproperty {{key}}='{{value}}' --nongui --testfile {{path/to/file}}.jmx`
