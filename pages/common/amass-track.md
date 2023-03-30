# amass track 
## chatgpt 
As an AI language model, I don't have access to your context or the specific technology you're referring to, but I can provide some general information on the command "amass track". 

1. "Amass": Amass is a popular open-source tool used for information gathering and reconnaissance in order to map out target networks. It utilizes a wide range of tools and techniques such as passive DNS, reverse WHOIS, and scraping tools to build this map. 

2. "Track": The word "track" usually refers to monitoring or following something over time. In the context of Amass, the "track" command likely instructs the tool to continuously monitor and update the map it has built, keeping track of any changes or new information that might become available.

Therefore, the "amass track" command likely tells Amass to actively monitor the target network, update the information as changes occur, and provide alerts or notifications when new information is gathered. 

## tldr 
 
> Track differences between enumerations of the same domain.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-track-subcommand>.

- Show the difference between the last two enumerations of the specified domain:

`amass track -dir {{path/to/database_directory}} -d {{domain_name}} -last 2`

- Show the difference between a certain point in time and the last enumeration:

`amass track -dir {{path/to/database_directory}} -d {{domain_name}} -since {{01/02 15:04:05 2006 MST}}`
