# snmpwalk 
## chatgpt 
snmpwalk is a command used to query SNMP-enabled network devices for information about their status and configuration. SNMP, or Simple Network Management Protocol, is a protocol used to manage and monitor network devices.

The snmpwalk command is used to walk through the MIB (Management Information Base) tree of a device, retrieving all the values of the variables. It returns a list of all the variables and their associated values in a hierarchical format.

Here is an example of a snmpwalk command:

```
snmpwalk -v 2c -c public 192.168.1.1
```

In this example, the options used are:

- `-v 2c` specifies that the SNMP version being used is version 2c.
- `-c public` specifies the community string used to authenticate access to the device. In this case, "public" is the community string. This is often a default community string used by many devices, so it is important to change it for security reasons.
- `192.168.1.1` is the IP address of the device being queried.

When the command is executed, it will return a list of all the variables and their associated values in a hierarchical format. The output can be quite extensive, so it is important to filter the output to only show the information that is relevant.

The snmpwalk command can be used in conjunction with other SNMP commands to manage and monitor network devices, such as snmpget and snmpset. 

## tldr 
 
> SNMP query tool.
> More information: <https://manned.org/snmpwalk>.

- Query the system information of a remote host using SNMPv1 and a community string:

`snmpwalk -v1 -c {{community}} {{ip}}`

- Query system information on a remote host by OID using SNMPv2 on a specified port:

`snmpwalk -v2c -c {{community}} {{ip}}:{{port}} {{oid}}`

- Query system information on a remote host by OID using SNMPv3 and authentication without encryption:

`snmpwalk -v3 -l {{authNoPriv}} -u {{username}} -a {{MD5|SHA}} -A {{passphrase}} {{ip}} {{oid}}`

- Query system information on a remote host by OID using SNMPv3, authentication, and encryption:

`snmpwalk -v3 -l {{authPriv}} -u {{username}} -a {{MD5|SHA}} -A {{auth_passphrase}} -x {{DES|AES}} -X {{enc_passphrase}} {{ip}} {{oid}}`

- Query system information on a remote host by OID using SNMPv3 without authentication or encryption:

`snmpwalk -v3 -l {{noAuthNoPriv}} -u {{username}} {{ip}} {{oid}}`
