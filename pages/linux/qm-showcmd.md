# qm showcmd 
## chatgpt 
I’m sorry, but as an AI language model, I don't have enough context to provide exact details. The command "qm showcmd" on its own doesn't refer to a specific operating system, programming language, or application, and there's no widely known command or tool with that name, that I’m aware of. 

Could you please provide additional information or context about the platform or the setting you are working in? This way, I can provide a more accurate explanation. 

## tldr 
 
> Show command line which is used to start the VM (debug info).
> More information: <https://pve.proxmox.com/pve-docs/qm.1.html>.

- Show command line for a specific virtual machine:

`qm showcmd {{vm_id}}`

- Put each option on a new line to enhance human readability:

`qm showcmd --pretty {{true}} {{vm_id}}`

- Fetch config values from a specific snapshot:

`qm showcmd --snapshot {{string}} {{vm_id}}`
