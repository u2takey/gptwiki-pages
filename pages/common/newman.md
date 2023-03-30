# newman 
## chatgpt 
Newman is a command line collection runner for Postman. It allows you to run a collection of API requests and execute tests as well as automate workflows involving API requests. The 'newman' command is used to execute these collections and can be used with several optional arguments to specify various settings or options. 

Here are some common uses of the 'newman' command with examples:

1. Running a collection file: To run a collection file using Newman, you need to specify the path of the file. 

```
newman run /path/to/collection.json
```

2. Running a collection using environment variables: You can specify environment variables to use in your collection by passing a path to an environment file with the -e parameter. 

```
newman run /path/to/collection.json -e /path/to/environment.json
```

3. Generating a report: You can generate a report after running your collection using the -r parameter. You can specify the format of the report by passing the type of the report to the parameter. 

```
newman run /path/to/collection.json -r html
```

Overall, the 'newman' command is a powerful tool for developers and testers who need to automate and test their API requests. It can be used to run collections of requests, execute tests, and generate reports, among other things. 

## tldr 
 
> Collection runner for Postman.
> More information: <https://github.com/postmanlabs/newman>.

- Run a collection (from a file):

`newman run {{path/to/collection.json}}`

- Run a collection (from a URL):

`newman run {{https://www.getpostman.com/collections/631643-f695cab7-6878-eb55-7943-ad88e1ccfd65-JsLv}}`
