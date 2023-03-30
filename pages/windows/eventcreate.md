# eventcreate 
## chatgpt 
The eventcreate command is a built-in command in the Windows operating system that allows the creation of custom events in the event viewer. It creates an event with the specified parameters in the specified event log.

Syntax:
eventcreate [/s Computer [/u Domain\User [/p Password]]] [/id EventID [/l Logfile]] [/t EventType] [/so SourceName] [/d Description]]

Parameters:
/s Computer : The remote system to create the event on.
/u Domain\User : The user context to create the event on.
/p Password : The password for the user account specified by the /u parameter.
/id EventID : The ID of the event to create.
/l Logfile : The name of the event log to create the event in.
/t EventType : The type of event to create (Information, Warning, Error, Success or Failure).
/so SourceName : The name of the source of the event.
/d Description : The description of the event.

Example:
The following command creates an informational event in the Application log with the Event ID of 1000 and a description of "Event created by user John Doe":

eventcreate /id 1000 /l Application /t Information /so MyApp /d "Event created by user John Doe" 

## tldr 
 
> Create custom entries in the event log.
> Event IDs can be any number between 1 and 1000.
> More information: <https://learn.microsoft.com/windows-server/administration/windows-commands/eventcreate>.

- Create a new event with a given ID (1-1000) in the log:

`eventcreate /t {{success|error|warning|information}} /id {{id}} /d "{{message}}"`

- Create an event in a specific event log:

`eventcreate /l {{log_name}} /t {{type}} /id {{id}} /d "{{message}}"`

- Create an event with a specific source:

`eventcreate /so {{source_name}} /t {{type}} /id {{id}} /d "{{message}}"`

- Create an event in a remote machine's event log:

`eventcreate /s {{hostname}} /u {{username}} /p {{password}} /t {{type}} /id {{id}} /d "{{message}}"`
