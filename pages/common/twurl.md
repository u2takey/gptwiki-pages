# twurl 
## chatgpt 
As an AI language model, I can explain about Twurl which is a command-line tool used for sending requests to the Twitter API.

Twurl is a program that uses a OAuth protocol to authenticate your Twitter credentials and then send HTTP requests to the Twitter API. It allows you to perform tasks like accessing specific user information, posting tweets, following or unfollowing other users, and so on.

Here are some of the key features of Twurl:

1. OAuth-based authentication: Twurl uses OAuth for authentication, which means you don't have to share your Twitter username and password with any third-party application.

2. Flexible API requests: Using Twurl, you can send HTTP requests to any endpoint of the Twitter API, including GET, POST, DELETE and more.

3. Customizable output: Twurl allows you to customize the output format of API responses using options like "-H" for headers, "-D" for data, and "-o" for output.

4. Supports multiple accounts: Twurl can handle multiple Twitter accounts by storing their access tokens and secrets in a configuration file.

Overall, Twurl is a useful tool for developers and power users who want to interact with the Twitter API from the command line. 

## tldr 
 
> Curl-like command but tailored specifically for the Twitter API.
> More information: <https://github.com/twitter/twurl>.

- Authorize `twurl` to access a Twitter account:

`twurl authorize --consumer-key {{twitter_api_key}} --consumer-secret {{twitter_api_secret}}`

- Make a GET request to an API endpoint:

`twurl -X GET {{twitter_api_endpoint}}`

- Make a POST request to an API endpoint:

`twurl -X POST -d '{{endpoint_params}}' {{twitter_api_endpoint}}`

- Upload media to Twitter:

`twurl -H "{{twitter_upload_url}}" -X POST "{{twitter_upload_endpoint}}" --file "{{path/to/media.jpg}}" --file-field "media"`

- Access a different Twitter API host:

`twurl -H {{twitter_api_url}} -X GET {{twitter_api_endpoint}}`

- Create an alias for a requested resource:

`twurl alias {{alias_name}} {{resource}}`
