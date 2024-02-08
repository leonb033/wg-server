# wg-server

This tool automates basic configuration of a wireguard server on Debian.
Setting up a nftables firewall with [debian_server_setup](https://github.com/leonb033/debian_server_setup) is required.

## Installation
`wget -O setup.sh https://raw.githubusercontent.com/leonb033/wg-server/main/setup.sh && bash setup.sh`

### Commands
#### wg-server setup
Creates a wg0 interface.

#### wg-server generate-keys
Generates new keys. All clients will be removed.

#### wg-server client-add
Adds a new client.

#### wg-server client-remove
Removes a client.
