# fastd 
## chatgpt 
fastd is a software program that provides a secure and efficient VPN (Virtual Private Network) solution. 

Fastd is designed to run on Linux operating systems and has been created with a focus on building scalable and robust VPN networks. The program is largely used by municipalities and communities to build secure connections between different locations that can be public or private. 

Fastd uses a variety of encryption techniques to provide secure communication, including ChaCha20, Poly1305, and Curve25519. It also offers features such as connection compression and increased packet throughput.

The fastd command is used to start, stop, or manage the fastd VPN software program. It offers options such as -c (config file), -d (debug mode), and -v (verbose mode) that allow for greater customization of the program's settings. These options are typically used by advanced users who need additional control over the VPN connection.

Overall, fastd is a powerful and secure VPN solution that offers a number of advanced features and configurations for those who need it. 

## tldr 
 
> VPN daemon.
> Works on Layer 2 or Layer 3, supports different encryption methods, used by Freifunk.
> More information: <https://fastd.readthedocs.io/en/stable/>.

- Start fastd with a specific configuration file:

`fastd --config {{path/to/fastd.conf}}`

- Start a Layer 3 VPN with an MTU of 1400, loading the rest of the configuration parameters from a file:

`fastd --mode {{tap}} --mtu {{1400}} --config {{path/to/fastd.conf}}`

- Validate a configuration file:

`fastd --verify-config --config {{path/to/fastd.conf}}`

- Generate a new key:

`fastd --generate-key`

- Show the public key to a private key in a configuration file:

`fastd --show-key --config {{path/to/fastd.conf}}`

- Show the current version::

`fastd -v`
