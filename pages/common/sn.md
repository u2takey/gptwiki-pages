# sn 
## chatgpt 
I’m sorry, but the command “sn” is ambiguous and can be interpreted in different ways depending on the context where it is used. It is possible that you might be referring to a specific operating system or software application where the command “sn” exists. Without additional information, I am not able to provide a precise explanation of the command. Could you please provide more details about the command or the context where it is used? 

## tldr 
 
> Mono StrongName utility for signing and verifying IL assemblies.
> More information: <https://manned.org/sn>.

- Generate a new StrongNaming key:

`sn -k {{path/to/key.snk}}`

- Re-sign an assembly with the specified private key:

`sn -R {{path/to/assembly.dll}} {{path/to/key_pair.snk}}`

- Show the public key of the private key that was used to sign an assembly:

`sn -T {{path/to/assembly.exe}}`

- Extract the public key to a file:

`sn -e {{path/to/assembly.dll}} {{path/to/output.pub}}`
