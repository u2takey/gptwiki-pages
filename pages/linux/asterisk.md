# asterisk 
## chatgpt 
Asterisk is a cross-platform, open-source software implementation of a telephone private branch exchange (PBX). The PBX functionality includes creating and maintaining extensions or endpoints, routing incoming and outgoing calls, voicemail, and other traditional PBX features. 

The command 'asterisk' is used to start the Asterisk service, which is typically installed on a server or a cloud-based virtual machine. The command is executed in a command-line interface, which could be the terminal window in Linux or PowerShell in Windows. 

When the command is executed, Asterisk starts running as a background process, and it listens to incoming requests and events, such as incoming calls, voicemail messages, or other communication signals. The command helps system administrators manage the Asterisk service by providing a set of CLI or graphical user interfaces through which they could configure the system, add new extensions or trunks, and monitor the system performance. 

Overall, the Asterisk command is a fundamental tool for anyone who wants to deploy, configure, or administer an Asterisk-based PBX system. 

## tldr 
 
> Telephone and exchange (phone) server.
> Used for running the server itself, and managing an already running instance.
> More information: <https://wiki.asterisk.org/wiki/display/AST/Home>.

- [R]econnect to a running server, and turn on logging 3 levels of [v]erbosity:

`asterisk -r -vvv`

- [R]econnect to a running server, run a single command, and return:

`asterisk -r -x "{{command}}"`

- Show chan_SIP clients (phones):

`asterisk -r -x "sip show peers"`

- Show active calls and channels:

`asterisk -r -x "core show channels"`

- Show voicemail mailboxes:

`asterisk -r -x "voicemail show users"`

- Terminate a channel:

`asterisk -r -x "hangup request {{channel_ID}}"`

- Reload chan_SIP configuration:

`asterisk -r -x "sip reload"`
