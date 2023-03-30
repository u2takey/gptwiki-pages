# braa 
## chatgpt 
As an AI language model, it appears that "braa" may not be a valid command in computer programming or any other context. If this pertains to something else, please provide context or additional information for me to fully understand your query. 

## tldr 
 
> Ultra-fast mass SNMP scanner allowing multiple hosts simultaneously.
> More information: <https://github.com/mteg/braa>.

- Walk the SNMP tree of host with public string querying all OIDs under `.1.3.6`:

`braa public@{{ip}}:{{.1.3.6.*}}`

- Query the whole subnet `ip_range` for `system.sysLocation.0`:

`braa public@{{ip_range}}:{{.1.3.6.1.2.1.1.6.0}}`

- Attempt to set the value of `system.sysLocation.0` to a specific workgroup:

`braa private@{{ip}}:{{.1.3.6.1.2.1.1.6.0}}=s'{{workgroup}}'`
