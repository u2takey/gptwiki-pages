# ohdear-cli 
## chatgpt 
OhDear-CLI is a command line interface tool that allows you to interact with the OhDear API. OhDear is a website monitoring and error tracking software that checks the uptime, performance, and security of your website or web application. 

OhDear-CLI provides a way to manage the features of the OhDear platform through a command line interface, without the need to log in to the website. With OhDear-CLI, you can add and remove sites, set up checks and notifications, and view reports and statistics.

To use OhDear-CLI, you need to install it first, which can be done via npm installation. Once installed, you can run the tool using the "ohdear-cli" command followed by the specific sub-command you want to execute. For example, if you want to create a new site in OhDear, you can run "ohdear-cli sites:create" command, which will prompt you to enter your API key and provide the details for the new site.

Overall, OhDear-CLI makes it easy to interact with the OhDear API, automate tasks, and monitor your website's health and performance. It is an excellent tool for developers, DevOps, and IT professionals who want to manage their website's monitoring and error tracking from the command line. 

## tldr 
 
> An unofficial Oh Dear CLI written with Laravel Zero.
> More information: <https://github.com/nunomaduro/ohdear-cli>.

- Display details about the currently authenticated user:

`ohdear-cli me`

- Add a new site to Oh Dear:

`ohdear-cli sites:add {{url}}`

- Display a list of sites and their current status:

`ohdear-cli sites:list`

- Display details about a specific site:

`ohdear-cli sites:show {{site_id}}`
