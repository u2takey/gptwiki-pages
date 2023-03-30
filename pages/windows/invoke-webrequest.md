# Invoke-WebRequest 
## chatgpt 
Invoke-WebRequest is a PowerShell cmdlet that allows users to programmatically send web requests to a website and receive the results. It is basically a command used to download data and content from the Internet. This cmdlet is used to retrieve information from web pages such as text, images, audio, video, etc.

The Invoke-WebRequest cmdlet can be used with a variety of HTTP methods – GET, POST, PUT, DELETE, and HEAD. It can also handle HTTPS requests and can even be used to authenticate users for specific websites. Some of the main features of this cmdlet include the ability to work with cookies, authentication, headers, and content types.

To execute an Invoke-WebRequest command, users need to specify the website URL and any additional parameters. For example, to download the content of a webpage, we can use the following command line:

`Invoke-WebRequest -Uri https://www.example.com`

This command will return the HTML content of the webpage specified by the URL.

Overall, the Invoke-WebRequest cmdlet is a powerful tool for web scraping and automated testing. It allows users to easily grab content from a web page and perform actions based on the results, all within a PowerShell command line environment. 

## tldr 
 
> Performs a HTTP/HTTPS request to the Web.
> This command can only be used through PowerShell.
> More information: <https://learn.microsoft.com/powershell/module/microsoft.powershell.utility/invoke-webrequest>.

- Download the contents of a URL to a file:

`Invoke-WebRequest {{http://example.com}} -OutFile {{path\to\file}}`

- Send form-encoded data (POST request of type `application/x-www-form-urlencoded`):

`Invoke-WebRequest -Method Post -Body @{ name='bob' } {{http://example.com/form}}`

- Send a request with an extra header, using a custom HTTP method:

`Invoke-WebRequest -Headers {{@{ X-My-Header = '123' }}} -Method {{PUT}} {{http://example.com}}`

- Send data in JSON format, specifying the appropriate content-type header:

`Invoke-WebRequest -Body {{'{"name":"bob"}'}}  -ContentType 'application/json' {{http://example.com/users/1234}}`

- Pass a username and password for server authentication:

`Invoke-WebRequest -Headers @{ Authorization = "Basic "+ [System.Convert]::ToBase64String([System.Text.Encoding]::ASCII.GetBytes("myusername:mypassword")) } {{http://example.com}}`
