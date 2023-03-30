# curlie 
## chatgpt 
I'm sorry, but "curlie" is not a valid command. It is possible that you might have misspelled the command or that it is not installed on your system. Can you please provide more information or context about where you came across this command so I can better assist you? 

## tldr 
 
> Curlie is a frontend to curl that adds the ease of use of httpie.
> More information: <https://github.com/rs/curlie>.

- Send a GET request:

`curlie {{httpbin.org/get}}`

- Send a POST request:

`curlie post {{httpbin.org/post}} {{name=john}} {{age:=25}}`

- Send a GET request with query parameters (e.g. `first_param=5&second_param=true`):

`curlie get {{httpbin.org/get}} {{first_param==5}} {{second_param==true}}`

- Send a GET request with a custom header:

`curlie get {{httpbin.org/get}} {{header-name:header-value}}`
