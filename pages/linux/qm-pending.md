# qm pending 
## chatgpt 
The "qm pending" command is a command used in the context of Queuing Managers (QM) in the IBM MQ messaging system. This command is used to list and display all pending messages waiting in a queue. 

When a message is sent in IBM MQ, it is placed in a queue until it is received by the intended recipient. If the recipient is unavailable, the message remains in the queue and is marked as pending. The "qm pending" command is used to view a list of all messages that are currently pending and waiting for delivery in the queue.

This command is useful in situations where you need to troubleshoot issues with message delivery or investigate why certain messages are not being received. By running "qm pending", you can see the number of pending messages, the name of the queue they are waiting in, and other details about the messages such as their size and priority.

Overall, the "qm pending" command is a helpful tool for managing and monitoring the flow of messages through IBM MQ queues. 

## tldr 
 
> Get the virtual machine configuration with both current and pending values.
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Get the virtual machine configuration of a specific virtual machine:

`qm pending {{vm_id}}`
