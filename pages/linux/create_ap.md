# create_ap 
## chatgpt 
The `create_ap` command is typically used in Linux-based operating systems and allows a user to create a wireless access point (AP) on a computer with a wireless network adapter. 

Here's a breakdown of the key components of the command:

`create_ap` - This is the main command that is used to create an access point.

`<interface>` - This specifies the wireless network adapter that will be used to create the access point. The interface argument could typically be `wlan0` on most systems.

`<SSID>` - This specifies the name of the access point that will be created. This is the name that other people will see when they search for a wireless network to connect to.

`<password>` - This is the password that will be set for the access point. Users will need this password to connect to the network.

`<internet_interface>` - This is the interface that will be used to provide internet access to the devices that connect to the access point. This could typically be `eth0` if your WiFi adapter is connected to the internet.

So, the full command may look something like this:

```
sudo create_ap wlan0 MyAP mypassword eth0
```

This command instructs the computer to create an access point using the `wlan0` wireless network adapter, named "MyAP", password "mypassword", and providing internet access through the `eth0` interface. The `sudo` keyword is used to specify that the command should be executed with root privileges, which may be required depending on your system configuration. 

## tldr 
 
> Create an AP (Access Point) at any channel.
> More information: <https://github.com/oblique/create_ap>.

- Create an open network with no passphrase:

`create_ap {{wlan0}} {{eth0}} {{access_point_ssid}}`

- Use a WPA + WPA2 passphrase:

`create_ap {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}`

- Create an access point without Internet sharing:

`create_ap -n {{wlan0}} {{access_point_ssid}} {{passphrase}}`

- Create a bridged network with Internet sharing:

`create_ap -m bridge {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}`

- Create a bridged network with Internet sharing and a pre-configured bridge interface:

`create_ap -m bridge {{wlan0}} {{br0}} {{access_point_ssid}} {{passphrase}}`

- Create an access port for Internet sharing from the same Wi-Fi interface:

`create_ap {{wlan0}} {{wlan0}} {{access_point_ssid}} {{passphrase}}`

- Choose a different Wi-Fi adapter driver:

`create_ap --driver {{wifi_adapter}} {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}`
