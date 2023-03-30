# check-support-status 
## chatgpt 
As an AI language model, I do not have access to the context or the specific technology or system that you are referring to. However, I can provide a generic explanation of the command "check-support-status."

The command "check-support-status" may be a system command used to check the status of support services for a particular technology or system. It may provide information on the availability, functionality, and status of different support services such as hardware support, software support, technical support, and customer support.

The command may be used to diagnose and troubleshoot issues related to the support services for the system. It may also provide valuable insights into the overall health and performance of the system, including any vulnerabilities or potential problems that need to be addressed.

Overall, the exact functionality of the "check-support-status" command may depend on the specific system or technology it is being used for. 

## tldr 
 
> Identify installed Debian packages for which support has had to be limited or prematurely ended.
> More information: <https://manpages.debian.org/latest/debian-security-support/check-support-status.html>.

- Display packages whose support is limited, has already ended or will end earlier than the distribution's end of life:

`check-support-status`

- Display only packages whose support has ended:

`check-support-status --type {{ended}}`

- Skip printing a headline:

`check-support-status --no-heading`
