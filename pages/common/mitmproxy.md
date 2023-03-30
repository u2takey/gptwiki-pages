# mitmproxy 
## chatgpt 
`mitmproxy` is an open-source tool used for intercepting, modifying, and inspecting network traffic. It is a man-in-the-middle proxy that enables users to monitor and manipulate network traffic flowing between two endpoints. It can be used for security testing, debugging, or monitoring of HTTP and HTTPS traffic.

To use `mitmproxy`, first, install it on your local system. Once installed, run the command `mitmproxy` on the terminal. This command will start the `mitmproxy` tool in the default mode, where it acts as a transparent proxy and intercepts all TLS and HTTP traffic.

You can also pass command-line arguments like -p, -P, -s, etc., to configure the tool as per your requirements. For example, you can use the `-p` option to specify the proxy port number where you want `mitmproxy` to listen for connections.

After starting `mitmproxy`, it will display a web interface where you can view and modify requests and responses in real-time. The web interface will show a list view of all intercepted traffic, and each traffic entry can be expanded to view more details like headers, request/response body, and timing information.

Overall, the `mitmproxy` tool is a powerful tool for debugging web apps, analyzing network traffic, and testing security vulnerabilities. It provides a rich set of features that enable developers, security researchers, and network administrators to inspect and manipulate network traffic in real-time. 

## tldr 
 
> An interactive man-in-the-middle HTTP proxy.
> More information: <https://mitmproxy.org>.

- Start mitmproxy with default settings:

`mitmproxy`

- Start mitmproxy bound to custom address and port:

`mitmproxy -b {{ip_address}} -p {{port}}`
