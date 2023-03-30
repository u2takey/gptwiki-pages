# grpcurl 
## chatgpt 
The `grpcurl` command is a command-line tool used to interact with remote gRPC servers using the protocol buffer (protobuf) format. The tool is mainly used for debugging and testing gRPC services without the need for a client library or language-specific dependencies.

The command accepts various options as input to establish a connection to the remote server following the format `grpcurl [options] <address> <service> <method>`. Here are some common options used:

- `-plaintext`: This option enables communication over an insecure plain-text connection

- `-cacert`, `-cert`, `-key`: These options set the path to the root CA, client certificate, and private key files respectively when using TLS.

- `-d`: This option sets the data to be sent in the request payload.

- `-import-path`, `-proto`: These options set the path to searched directories for .proto files and the path to the .proto files themselves respectively.

- `-H`: This option sets the request header.

- `-v`: This option sets the verbosity level of the output.

For example, a typical `grpcurl` command to invoke the `ListUsers` method on a remote gRPC server using the plaintext protocol would look like this:

```
grpcurl -plaintext myserver:8080 mypackage.UserService/ListUsers
```
Here, "`myserver:8080`" specifies the IP address or DNS name and port number where the server is running, "`mypackage.UserService`" is the fully qualified name of the gRPC service, and "`ListUsers`" is the name of the method to call.

When executed, the command sends a request to the server and waits for a response. The output shows the response received from the server, including status, headers, and the message payload, according to the verbosity level set by the user. 

## tldr 
 
> Like cURL, but for gRPC: CLI tool for interacting with gRPC servers.
> More information: <https://github.com/fullstorydev/grpcurl>.

- Send an empty request:

`grpcurl {{grpc.server.com:443}} {{my.custom.server.Service/Method}}`

- Send a request with a header and a body:

`grpcurl -H "{{Authorization: Bearer $token}}" -d {{'{"foo": "bar"}'}} {{grpc.server.com:443}} {{my.custom.server.Service/Method}}`

- List all services exposed by a server:

`grpcurl {{grpc.server.com:443}} list`

- List all methods in a particular service:

`grpcurl {{grpc.server.com:443}} list {{my.custom.server.Service}}`
