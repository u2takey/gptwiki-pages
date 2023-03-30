# tea 
## chatgpt 
I'm sorry, as an AI language model, I cannot execute commands as I am just a text generation software. However, I can explain to you about the term "tea."

Tea is a hot beverage usually made from the leaves of the tea plant, Camellia sinensis, although it can also be made from other plants such as mint or chamomile. Tea is typically served hot, though it can also be served cold, and it is enjoyed in various cultures around the world. 

There are many different types of tea, each with its unique flavor, aroma, and health benefits. Some of the popular tea varieties include green tea, black tea, oolong tea, white tea, herbal tea, and flavored tea. The method of preparing tea varies depending on the type of tea and the preferences of the tea drinker. 

In a broader context, "tea" can also refer to a gathering or social event in which tea is served and enjoyed among a group of people. Such gatherings often involve the use of specialized teapots, cups, and other accessories to enhance the tea-drinking experience. 

## tldr 
 
> A command-line tool to interact with Gitea servers.
> More information: <https://gitea.com/gitea/tea>.

- Log into a Gitea server:

`tea login add --name "{{name}}" --url "{{url}}" --token "{{token}}"`

- Display all repositories:

`tea repos ls`

- Display a list of issues:

`tea issues ls`

- Display a list of issues for a specific repository:

`tea issues ls --repo "{{repository}}"`

- Create a new issue:

`tea issues create --title "{{title}}" --body "{{body}}"`

- Display a list of open pull requests:

`tea pulls ls`

- Open the current repository in a browser:

`tea open`
