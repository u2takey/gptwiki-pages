# doctl serverless 
## chatgpt 
The `doctl serverless` command is used with the DigitalOcean Command Line Interface (CLI) tool to manage serverless functions on DigitalOcean's App Platform.

In more detail:

- `doctl` is a command-line tool that allows developers to manage their DigitalOcean resources from the terminal.
- `serverless` is a subset of the `doctl` command-line tool that focuses on managing serverless functions on DigitalOcean's App Platform.
- The App Platform is a fully-managed platform that allows developers to build, deploy, and scale their applications and services quickly and easily.

Using the `doctl serverless` command, developers can create, list, update, and delete their serverless functions on the App Platform. They can also view logs, metrics, and other details related to their functions. 

## tldr 
 
> Manage serverless functions.
> More information: <https://docs.digitalocean.com/reference/doctl/reference/serverless/>.

- Connect local serverless support to a functions namespace:

`doctl serverless connect`

- Deploy a functions project to your functions namespace:

`doctl serverless deploy`

- Obtain metadata of a functions project:

`doctl serverless get-metadata`

- Provide information about serverless support:

`doctl serverless status`
