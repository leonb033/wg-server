# wg-server

This tool automates configuration of wireguard interfaces on Debian.

## Requirements
- Debian 12
- wireguard
- wireguard-tools

## Installation
`wget -O setup.sh https://raw.githubusercontent.com/leonb033/wg-server/main/setup.sh && bash setup.sh`

## Commands
### wg-server \<INTERFACE\> create
Sets up a new wireguard interface.

### wg-server \<INTERFACE\> delete
Deletes this wireguard interface.

### wg-server \<INTERFACE\> generate-keys
Generates new public and private key for this interface.

### wg-server \<INTERFACE\> add-peer
Adds a new peer to this interface.

### wg-server \<INTERFACE\> remove-peer
Removes a peer from this interface.

## Useful wireguard commands:
### sudo wg show
List all running wireguard interfaces.

### sudo systemctl [start/stop] wg-quick@\<INTERFACE\>.service
Start / stop this interface service.

### sudo systemctl [enable/disable] wg-quick@\<INTERFACE\>.service
Enable / disable autostart for this interface service.
