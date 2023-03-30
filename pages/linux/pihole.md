# pihole 
## chatgpt 
Pihole is a command used to manage and configure the Pi-hole network-level advertisement and internet tracker blocker for a home network. It is a software solution that works by blocking domain names that are known to be used by advertisers, trackers or malware. 

The Pi-hole software is designed to be run on a Raspberry Pi, but it can be installed on other platforms like Ubuntu, Debian, or CentOS. Once installed, it can be used to block ads for every device connected to your home network including smartphones, smart TVs and computers.

Some of the options and features that can be configured using the pihole command include:

- Updating the blacklists of domain names to be blocked
- Viewing the status of the Pi-hole service
- Whitelisting domain names that should not be blocked
- Viewing statistics and logs about the blocked domain names and queries
- Changing the DNS server used by the Pi-hole service.

Overall, the pihole command is a powerful tool that can significantly reduce or even eliminate ads, trackers and potential malware links from your online experience, making it a useful addition to any home network. 

## tldr 
 
> Terminal interface for the Pi-hole ad-blocking DNS server.
> More information: <https://docs.pi-hole.net/core/pihole-command/>.

- Check the Pi-hole daemon's status:

`pihole status`

- Update Pi-hole and Gravity:

`pihole -up`

- Monitor detailed system status:

`pihole chronometer`

- Start or stop the daemon:

`pihole {{enable|disable}}`

- Restart the daemon (not the server itself):

`pihole restartdns`

- Whitelist or blacklist a domain:

`pihole {{whitelist|blacklist}} {{example.com}}`

- Search the lists for a domain:

`pihole query {{example.com}}`

- Open a real-time log of connections:

`pihole tail`
