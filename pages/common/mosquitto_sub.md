# mosquitto_sub 
## chatgpt 
Mosquitto_sub is a command-line utility that is used to subscribe to MQTT topics and receive messages from the MQTT broker. MQTT (Message Queue Telemetry Transport) is a lightweight publish-subscribe network protocol that is used to send messages between devices over the internet.

The mosquitto_sub command is used to connect to an MQTT broker and start receiving messages that are published to the specified topics. It is part of the Mosquitto MQTT broker software package, which also includes mosquitto_pub, an MQTT client that is used to publish messages to the MQTT broker.

Syntax:
`mosquitto_sub [-h host] [-p port] [-u username] [-P password] [-t topic]`

Here is the explanation of the parameters used in the mosquitto_sub command:

- `-h host`: This parameter is used to specify the hostname or IP address of the MQTT broker that you want to connect to. If not specified, the default hostname is localhost.
- `-p port`: This parameter is used to specify the port number of the MQTT broker. The default port number is 1883 for non-SSL connections and 8883 for SSL connections.
- `-u username`: This parameter is used to specify the username that you want to use to connect to the MQTT broker. If the MQTT broker requires authentication, you must specify a valid username.
- `-P password`: This parameter is used to specify the password that you want to use to connect to the MQTT broker. If the MQTT broker requires authentication, you must specify a valid password.
- `-t topic`: This parameter is used to specify the topic(s) that you want to subscribe to. You can specify multiple topics by separating them with a comma. If you do not specify any topics, you will receive messages from all topics.

Once you have specified the required parameters, you can execute the mosquitto_sub command. The command will connect to the MQTT broker and start receiving messages that are published to the specified topics. The messages will be displayed in the terminal as they are received, along with some additional information such as the topic name, message payload, and QoS level. The mosquitto_sub command will continue running and receiving messages until you terminate it by pressing Ctrl+C. 

## tldr 
 
> A simple MQTT version 3.1.1 client that will subscribe to topics and print the messages that it receives.
> More information: <https://mosquitto.org/man/mosquitto_sub-1.html>.

- Subscribe to the topic `sensors/temperature` information with Quality of Service (`QoS`) set to 1. (The default hostname is `localhost` and port 1883):

`mosquitto_sub -t {{sensors/temperature}} -q {{1}}`

- Subscribe to all broker status messages publishing on `iot.eclipse.org` port 1885 and print published messages verbosely:

`mosquitto_sub -v -h "iot.eclipse.org" -p 1885 -t {{\$SYS/#}}`

- Subscribe to multiple topics matching a given pattern. (+ takes any metric name):

`mosquitto_sub -t {{sensors/machines/+/temperature/+}}`
