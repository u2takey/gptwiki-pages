# birdc 
## chatgpt 
The "birdc" command is a command-line tool that is used to manage the BIRD Internet routing daemon. The BIRD daemon is a routing software that is used to manage and exchange routes between different networks.

The "birdc" command is used to access the BIRD control interface, which allows the administrator to manage and configure the BIRD daemon. Once the command is executed, a prompt will appear allowing the administrator to enter different commands to perform specific tasks.

Some of the tasks that can be performed using the "birdc" command include querying the routing tables, modifying the routing policies, and configuring the BIRD daemon itself.

Here are some examples of the most commonly used "birdc" commands:

- "show route": used to display the current routing table
- "show protocols": used to display the status of all the routing protocols configured on BIRD
- "enable [protocol]": used to enable a specific routing protocol
- "disable [protocol]": used to disable a specific routing protocol
- "configure terminal": used to enter the configuration mode and edit the BIRD configuration file
- "quit": used to exit the birdc control interface. 

## tldr 
 
> Bird remote control.
> Command tool to retrieve information like routes from bird and perform configurations during runtime.
> More information: <https://bird.network.cz/>.

- Open the remote control console::

`birdc`

- Reload the configuration without restarting Bird:

`birdc configure`

- Show the current status of Bird:

`birdc show status`

- Show all active protocols:

`birdc show protocols`

- Show all details about a protocol:

`birdc show protocols {{upstream1}} all`

- Show all routes that contain a specific AS number:

`birdc "show route where bgp_path ~ [{{4242120045}}]"`

- Show all best routes:

`birdc show route primary`

- Show all details of all routes from a given prefix:

`birdc show route for {{fd00:/8}} all`
