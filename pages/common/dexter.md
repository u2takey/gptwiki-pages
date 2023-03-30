# dexter 
## chatgpt 
I'm sorry, as an AI language model, I need more details to understand which command you are referring to. Can you provide more context or specific information about the command "dexter"? 

## tldr 
 
> Tool for authenticating the kubectl users with OpenId Connect.
> More information: <https://github.com/gini/dexter>.

- Create and authenticate a user with Google OIDC:

`dexter auth -i {{client_id}} -s {{client_secret}}`

- Override the default kube config location:

`dexter auth -i {{client_id}} -s {{client_secret}} --kube-config {{sample/config}}`
