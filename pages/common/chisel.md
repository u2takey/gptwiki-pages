# chisel 
## chatgpt 
Chisel is a command-line tool used in Verilog, SystemVerilog, and VHDL designs to generate digital logic designs using a high-level hardware construction language. It allows a designer to write RTL (register-transfer level) code that can be synthesized into lower-level hardware, such as FPGA or ASIC designs.

Chisel is used to build hardware description languages (HDLs) that can describe complex digital circuits with a high level of abstraction. It uses a Scala-based syntax to generate code and supports object-oriented features, allowing for modular and reusable hardware designs.

Chisel can also generate C++ code using the FIRRTL hardware intermediate representation, providing a flexible and efficient way of designing digital circuits.

Some of the key features of Chisel include:

1. High-level hardware construction language
2. Reusability of design blocks
3. Support for multi-language interoperability
4. Faster design iteration
5. Scalable design methodology
6. Automatic design space exploration and tuning

Overall, Chisel is a powerful tool that enables designers to create complex digital circuits using a high-level hardware construction language, facilitating a more efficient and streamlined design process. 

## tldr 
 
> Create TCP tunnels. Includes both client and server.
> More information: <https://github.com/jpillora/chisel>.

- Run a Chisel server:

`chisel server`

- Run a Chisel server listening to a specific port:

`chisel server -p {{server_port}}`

- Run a chisel server that accepts authenticated connections using username and password:

`chisel server --auth {{username}}:{{password}}`

- Connect to a Chisel server and tunnel a specific port to a remote server and port:

`chisel client {{server_ip}}:{{server_port}} {{local_port}}:{{remote_server}}:{{remote_port}}`

- Connect to a Chisel server and tunnel a specific host and port to a remote server and port:

`chisel client {{server_ip}}:{{server_port}} {{local_host}}:{{local_port}}:{{remote_server}}:{{remote_port}}`

- Connect to a Chisel server using username and password authentication:

`chisel client --auth {{username}}:{{password}} {{server_ip}}:{{server_port}} {{local_port}}:{{remote_server}}:{{remote_port}}`
