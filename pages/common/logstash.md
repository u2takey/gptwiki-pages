# logstash 
## chatgpt 
Logstash is an open-source data processing pipeline tool that allows you to collect, process and forward huge amounts of log data in real time. It is primarily used to collect and ship logs from different sources into various destinations, such as Elasticsearch, Kafka, or Amazon S3.

The logstash command is used to run, configure, and manage Logstash. When you execute the logstash command, Logstash will start running in the background and listen for incoming logs from various sources. It accepts inputs from a variety of sources such as syslog messages, CSV data, HTTP requests, and many others. Once it receives data, it will parse and transform it into the format that your output destination can understand.

To use the logstash command, you first need to create a configuration file that defines the input, filter, and output plugins that you want to use. The configuration file is typically a YAML file that specifies all the settings and options for each plugin. Once you have created the configuration file, you can run the logstash command and specify the location of the configuration file as an argument.

For example, to run Logstash with a configuration file located at /etc/logstash/conf.d/myconfig.yml, you can use the following command:

```
logstash -f /etc/logstash/conf.d/myconfig.yml
```

The above command will start Logstash and load the configuration file myconfig.yml, which will tell Logstash which inputs to listen to, which filters to apply, and where to send the output data. You can add additional options to this command to customize the behavior of Logstash, such as setting the number of worker threads or specifying logging settings.

Overall, the logstash command is a versatile tool that allows you to configure and run Logstash with ease, making it a powerful solution for processing and analyzing log data. 

## tldr 
 
> An Elasticsearch ETL (extract, transform and load) tool.
> Commonly used to load data from various sources (such as databases and log files) into Elasticsearch.
> More information: <https://www.elastic.co/products/logstash>.

- Check validity of a Logstash configuration:

`logstash --configtest --config {{logstash_config.conf}}`

- Run Logstash using configuration:

`sudo logstash --config {{logstash_config.conf}}`

- Run Logstash with the most basic inline configuration string:

`sudo logstash -e 'input {} filter {} output {}'`
